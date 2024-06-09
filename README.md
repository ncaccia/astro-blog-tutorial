# Astro.build Tutorials

## Build a blog - Learnings

#### Unit 1: Setting up enviroment

- Deploying on https://netlify.com
  - https://app.netlify.com/teams/ncaccia
  - [Step by step: how to deploy on netlify](https://www.netlify.com/blog/2016/09/29/a-step-by-step-guide-deploying-on-netlify/)

#### Unit 2 - Pages

- .astro syntax === html + js files
  - `.astro` file’s frontmatter is written in JS
- [File-based Routing in Astro](https://docs.astro.build/en/basics/astro-pages/#file-based-routing)
- [Astro page HTML](https://docs.astro.build/en/basics/astro-pages/#astro-pages)
- Write Markdown content
  - frontmatter: information at the top of the file, inside the code fences === data—including tags and a post image—is information about your post that Astro can use.
- Add dynamic content about you
  - Define variables in your Astro script using JavaScript or TypeScript expressions.
  - Use these variables in your Astro template inside curly braces { } to tell Astro you’re using some JavaScript.
  - Writing an Astro template is very much like writing HTML, but you can include JavaScript expressions within it.
  - The Astro frontmatter script contains only JavaScript.
  - You can use all modern JavaScript logical operators, expressions and functions in either section of your .astro file. But, curly braces are necessary (only) in the HTML template body.
  -
- Conditionally render elements

  - Astro’s templating syntax is similar to [JSX syntax](https://react.dev/learn/writing-markup-with-jsx).
  - Logical AND (&&) Operator: Used for conditional rendering where the component is rendered only if the condition is true. Ex: `{happy && <p>I am happy to be learning Astro!</p>}`

- **Style an individual page**
  - Astro’s own <style></style> tags, you can style items on your page. Adding attributes and directives to these tags gives you even more ways to style.
  - using CSS variables: The Astro <style> tag can also reference any variables from your frontmatter script using the define:vars={ {...} } directive. You can define variables within your code fence, then use them as CSS variables in your style tag.
    - add a variable attribute to the sytle tag: `<style define:vars={{anyVariable}}>`
    - [Astro syntax vs JSX - comparison](https://docs.astro.build/en/basics/astro-syntax/#differences-between-astro-and-jsx)
    - [Astro <style> tag](https://docs.astro.build/en/guides/styling/#styling-in-astro)
    - [CSS variables in Astro](https://docs.astro.build/en/guides/styling/#css-variables)
- **Add a global stylesheet**
  - create `src/styles/global.css` and import it on the frontmatter section

#### Unit 3 - Components

- 
