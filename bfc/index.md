The phrase "a box's containing block" means "the containing block in which the box lives," not the one it generates.

 The 'display' property, specifies a box's type.

 The following values of the 'display' property make an element block-level: 'block', 'list-item', and 'table'.

The three terms "block-level box," "block container box," and "block box" 

In other words: if a block container box (such as that generated for the DIV above) has a block-level box inside it (such as the P above), then we force it to have only block-level boxes inside it.

inline-block:
This value causes an element to generate an inline-level block container. The inside of an inline-block is formatted as a block box, and the element itself is formatted as an atomic inline-level box.