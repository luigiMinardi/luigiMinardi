[Original gist](https://gist.github.com/luigiMinardi/4574708d404cdf4fe0da7ac6fe2314db)

# $$\color{#D29922}\textsf{\Large\&#x26A0;\kern{0.2cm}\normalsize Warning}$$ 
## $$\textsf{Github released Tex support and colors* to the markdown and you din't realized}$$

$\normalsize{\textsf{*You can use Tex to produce colors, but the real objective of it is to write math so it is more of a workaround that works good enought.}}$  

$\color{#58A6FF}\textsf{\large\&#x24D8;\kern{0.2cm}\normalsize Note}$ Somethings are different here on `gist` and on the actual markdown of README's on github or the markdown of issues, etc.

### Table of contents
* [Warnings & Notes](#warnings-and-notes)  
* [Learn Tex basic syntax](#tex)  
$\to$  [Text in Tex](#text-in-tex)  
$\to$  [Font Styles](#font-styles)  
$\to$  [Colors](#colors)  
$\to$  [Font Sizes](#font-sizes)  
* [Tex limitations](#colorred-textsftex-limitations)
* [Color examples table](#table-with-some-color-examples)
* [Useful links](#useful-links)

## Warnings and Notes

To do the warning and note on the `github markdown` is that way:
```
__Warning__
__Note__
```
__Warning__
__Note__  

On the `gist` markdown you need to use the Tex syntax this way:
```
$\color{#D29922}\textsf{\Large\&#x26A0;\kern{0.2cm}\normalsize Warning}$ 
$\color{#58A6FF}\textsf{\Large\&#x24D8;\kern{0.2cm}\normalsize Note}$
```
$\color{#D29922}\textsf{\Large\&#x26A0;\kern{0.2cm}\normalsize Warning}$ 
$\color{#58A6FF}\textsf{\Large\&#x24D8;\kern{0.2cm}\normalsize Note}$

To learn the syntax of `Tex` you can look at the `Katex` [docs](https://katex.org/docs/supported.html), you can also check the [sorted docs](https://katex.org/docs/support_table.html).  

`Katex` are not exacly `Tex`, but their docs are very well made and easy to understand, also most features of one are in the other. And the syntax is the same.

# Tex
To start writting with Tex syntax you need to use `$` at the start and end of the text. `$foo$`.
> $foo$  

If you want to centralize you can put 2 `$`. `$$foo$$` is a centralized text.
> $$foo$$

## Text in Tex
I prefer to write text in tex using the `\text{foo}` but you have other ways to do it as you can see bellow.  

#####  Without anything
$lorem ipsum dolor sit amet$  
```bash
$lorem ipsum dolor sit amet$
```

##### With `\text` alone
$\text lorem ipsum dolor sit amet$
```bash
$\text lorem ipsum dolor sit amet$
```

#####  With `\text{}`
$\text{lorem ipsum dolor sit amet}$
```bash
$\text{lorem ipsum dolor sit amet}$
```

##### Using `\ ` to add spaces (` `)
$lorem\ ipsum\ dolor\ sit\ amet$
```bash
$lorem\ ipsum\ dolor\ sit\ amet$
```

##### Using `\text` without `{}` and with `\ ` to add spaces
$\text lorem\ ipsum\ dolor\ sit\ amet$
```bash
$\text lorem\ ipsum\ dolor\ sit\ amet$
```

## Font Styles

To change the font style you need to add suffixes to the `\text`.  

|suffix|   syntax  |          command         |          result         |
| ---  |    ---    |            ---           |           ---           |
`none` |  `\text`  |  `$\text{lorem ipsum}$`  | $\text{lorem ipsum}$
`\rm`  | `\textrm` | `$\textrm{lorem ipsum}$` | $\textrm{lorem ipsum}$
`\sf`  | `\textsf` | `$\textsf{lorem ipsum}$` | $\textsf{lorem ipsum}$
`\bf`  | `\textbf` | `$\textbf{lorem ipsum}$` | $\textbf{lorem ipsum}$
`\up`  | `\textup` | `$\textup{lorem ipsum}$` | $\textup{lorem ipsum}$
`\tt`  | `\texttt` | `$\texttt{lorem ipsum}$` | $\texttt{lorem ipsum}$
`\it`  | `\textit` | `$\textit{lorem ipsum}$` | $\textit{lorem ipsum}$

## Colors
To use colors you can use `\color` or `\textcolor`.  
You can also use background colors with `\colorbox` or `\fcolorbox` if you also want a color border (`fcolorbox` uses 2 params `{}`).

|                        command                        |                           result                      |
|                          ---                          |                            ---                        |
`$\color{red}{\textsf{lorem ipsum}}$`                   | $\color{red}{\textsf{lorem ipsum}}$
`$\color{#f00}{\textsf{lorem ipsum}}$`                  | $\color{#f00}{\textsf{lorem ipsum}}$ 
`$\color{rgb(255,0,0)}{\textsf{lorem ipsum}}$`          | $\color{rgb(255,0,0)}{\textsf{lorem ipsum}}$
`$\color{rgba(255,0,0, 0.4)}{\textsf{lorem ipsum}}$`    | $\color{rgba(255,0,0, 0.4)}{\textsf{lorem ipsum}}$
`$\color{hsl(0,100%,50%)}{\textsf{lorem ipsum}}$`       | $\color{hsl(0,100%,50%)}{\textsf{lorem ipsum}}$
`$\color{hsla(0,100%,50%, 0.4)}{\textsf{lorem ipsum}}$` | $\color{hsla(0,100%,50%, 0.4)}{\textsf{lorem ipsum}}$
`$\textcolor{red}{\textsf{lorem ipsum}}$`               | $\textcolor{red}{\textsf{lorem ipsum}}$
`$\colorbox{red}{\textsf{lorem ipsum}}$`                | $\colorbox{red}{\textsf{lorem ipsum}}$
`$\fcolorbox{yellow}{red}{\textsf{lorem ipsum}}$`       | $\fcolorbox{yellow}{red}{\textsf{lorem ipsum}}$

## Font Sizes

|                command              |                result              |
|                  ---                |                 ---                |
`$\Huge{\textsf{lorem ipsum}}$`       | $\Huge{\textsf{lorem ipsum}}$
`$\huge{\textsf{lorem ipsum}}$`       | $\huge{\textsf{lorem ipsum}}$
`$\LARGE{\textsf{lorem ipsum}}$`      | $\LARGE{\textsf{lorem ipsum}}$
`$\Large{\textsf{lorem ipsum}}$`      | $\Large{\textsf{lorem ipsum}}$
`$\large{\textsf{lorem ipsum}}$`      | $\large{\textsf{lorem ipsum}}$
`$\normalsize{\textsf{lorem ipsum}}$` | $\normalsize{\textsf{lorem ipsum}}$
`$\small{\textsf{lorem ipsum}}$`      | $\small{\textsf{lorem ipsum}}$
`$\scriptsize{\textsf{lorem ipsum}}$` | $\scriptsize{\textsf{lorem ipsum}}$
`$\tiny{\textsf{lorem ipsum}}$`       | $\tiny{\textsf{lorem ipsum}}$

## $\color{red}{ \textsf{Tex limitations}}$

The problem with writting using tex is that you can't select the text as you can se with the title above witten with Tex. (You can copy the `Tex Commands` with the right button of the mouse, but it isn't as good as it could be.)

You also have limited characters per line (at least here on `gist` as of today) or it'll break some way.

<details>

<summary>Example of Tex breaking creating a horizontal bar</summary>

$\text{Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.}$

</details>

AS you can se, [$Tex breaks inside  links$](#colorred-textsftex-limitations) too. (using `[]()` here)

<a href="#colorred-textsftex-limitations">
  $\textsf{Tex inside an a tag}$
</a>  

$\textsf{Tex outside an a tag}$

## Table with some color examples

| $\color{black}{\textsf{Black}}$ |  $\color{blue}{\textsf{Blue}}$ | $\color{brown}{\textsf{Brown}}$ | $\color{darkgray}{\textsf{Dark Gray}}$  | $\color{gray}{\textsf{Gray}}$ | 
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| $\color{lightgray}{\textsf{Light Gray}}$ |  $\color{green}{\textsf{Green}}$ | $\color{lightblue}{\textsf{Light Blue}}$ | $\color{lime}{\textsf{Lime}}$  | $\color{magenta}{\textsf{Magenta}}$ |
| $\color{olive}{\textsf{Olive}}$ |  $\color{orange}{\textsf{Orange}}$ | $\color{pink}{\textsf{Pink}}$ | $\color{purple}{\textsf{Purple}}$  | $\color{red}{\textsf{Red}}$ | 
| $\color{teal}{\textsf{Teal}}$ |  $\color{violet}{\textsf{Violet}}$ | $\color{white}{\textsf{White}}$ | $\color{yellow}{\textsf{Yellow}}$  | $\color{BurntOrange}{\textsf{Burnt Orange}}$ |
| $\small{ \color{white} \colorbox{Green}{ \textsf{White on Green}}}$   | $\color{pink} \fcolorbox{teal}{blue}{ \textsf{ \small{Pink on Blue w/ teal border}}}$  | $\color{black} \fcolorbox{white}{red}{ \small{ \textsf{Black on Red w/ white border}}}$   | $\color{black} \fcolorbox{red}{white}{ \small{ \textsf{Black on White w/ red border}}}$ | $\color{black} \colorbox{BurntOrange}{ \small{ \textsf{Black on Orange}}}$ |
| $\color{purple} \colorbox{olive}{ \textsf{Purple on Olive}}$ |  $\color{green} \colorbox{white}{ \textsf{Green on White}}$ | $\color{Orange} \fcolorbox{blue}{black}{ \textsf{Orange on Black w/ blue border}}$  | $\color{blue} \small{ \fcolorbox{lime}{white}{ \textsf{Blue on White w/ lime border}}}$ | $\color{lime} \colorbox{violet}{ \textsf{Lime on Violet}}$ |

# Useful links

* [MathJax Github](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)  
* [Github Markup request colors thread (issue 1440)](https://github.com/github/markup/issues/1440)
* [LaTex Wiki](https://en.wikibooks.org/wiki/LaTeX/Mathematics)
* [KaTex Wiki](https://katex.org/docs/supported.html)
* [The TeX Users Group (TUG)](https://tug.org)

