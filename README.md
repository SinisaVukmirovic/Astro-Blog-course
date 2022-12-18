## Astro Blog course
___

#### You can use normal JavaScript within { curly brackets } 

### Astro uses JSX-like syntax, when returning its with parenthesis => () instead of curly brackets => {} notation

#### There is a top-level AWAIT in top --- section

##### Anything inside "public" folder is untouched by Astro, it is basically at the root of the server and can be referenced just by this /.. for example "/favicon.svg"

#### Styles in AStro are scope to the components and Astro also uses :where selector which strips of all CSS specificity

##### Adding is:global attribute to the style tag element, will make that styles global 
##### Adding lang="sass" attribut to the style tag, lets us use SCSS/SASS language 
#### Adding define:vars attribute with ={{ someDynamicVar, anotherDynamicVar }} lets us define variable inside of CSS, with values defined in JS, so they can later be manipulated and changed if needed 

### class:list in Astro and conditional classes
```
    const isRed = true;

	<p class:list={["big", {red: isRed}]}>defined variable colors</p>

    .big {
		font-size: 3rem;
	}
	.red {
		color: red;
	}
```