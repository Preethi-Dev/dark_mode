# Dark_mode✨

Hey There, Most of the users(specially developers) are the huge fan of dark mode and try to use it on all apps and software.
They will definitely expect enabling dark mode on web content also. So, we can get their theme preference by their OS(In this blog, technically call as "UA" means User Agent) without need to toggle😲😲.

![dark/light mode image](/asset/light_dark_mode.png)

>***We can achieve these without asking help to JavaScript🎉 which really sounds good (Disclaimer: I'm not mean JS is complicated, But we enable these feature as simple as possible).***

## A magical media query🪄
Using 
### @media (prefers-color-scheme: dark) media query,
We can detect if the user has requested a light or dark color theme by User Agent(based on OS settings).

```
@media (prefers-color-scheme: dark) {
  :root {
    --main-bg-color: #040404;
    --card-bg-color: #3a3a38;
    --icon-bg-color: #f7d1a2;
    --main-light-onColor: #aeb4bd;
    --main-dark-onColor: #777676;
  }
}

/* we can also style for light mode*/
@media (prefers-color-scheme: dark) {
}
```
### You can experiment with [Live Demo](https://preethi-dev.github.io/Claymorphism/).

