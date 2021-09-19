# Example

```
<List>
  <ListItem>Item 1</ListItem>
  <ListItem>Item 2</ListItem>
  <ListItem>Item 3</ListItem>
</List>
```

<Playground>
  import React, {useCallback} from 'react'

    export default () => {
    	const onClick = useCallback(() => {
    		alert('Oh yeah')
    	}, [])

    	return (
    		<>
    			<blockquote cite="https://en.wikipedia.org/wiki/Rose_is_a_rose_is_a_rose_is_a_rose">A <span className="rose">rose</span> is a <span className="rose">rose</span> is a <span className="rose">rose</span>.</blockquote>
    			<my.Button onClick={onClick}>It's all coming together</my.Button>
    		</>
    	)
    }

</Playground>

# Properties

| Component | Property    | Description                                      | Default    |
| --------- | ----------- | ------------------------------------------------ | ---------- |
| ListItem  | `indicator` | Which indicator is to be displayed for the item. | `"bullet"` |
