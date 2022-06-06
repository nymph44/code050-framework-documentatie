# code050 UI kit
---
| Version  |1.0|
|---------|------------|
| Total Components | 18 |
| License | private |
| Last commit | May 29 2022|

[Official website](https://www.code050.nl)

[Components](https://www.code050.nl)

[How to use](https://www.code050.nl)

---
**The code050 UI kit works by calling onto the blade components inside Laravel. I tried my best to make these components as extensive as possible by making use of ability to fill them with props.**

It's easy, reusable, and reliable.

---
## Features
* Consistency inside the Code050 ecosystem
* Cleaner code
* Reusability

---
## Install now!

The simplest and fastest way to get up and running with the Code050 UI kit is by cloning the repo.

> Recommend creating a components folder inside resources

    root directory / resources / views / components

!> Currently not as a package available! Clone the repo into your project.

```git
git clone https://github.com/nymph44/code050-framework-documentatie.git
```

## Fonts
The Code050 UI kit was designed with the Raleway and Nunito font in mind. So be sure to follow these instructions. For instance, via Google Web Fonts:

```style
<link href='https://fonts.googleapis.com/css?family=Raleway' rel='stylesheet'>
```

## Font icons
To use the font Icon component, you must first add the Font Awesome Icons font. Here are some instructions on how to do so:
```npm
npm install --save @fortawesome/fontawesome-free
```

> In order to to fully use the framework you need to install Daisy UI and Flowbite to make use of the required plugins.
```npm
npm i Daisyui
```

```npm
npm i flowbite
```
```npm
npm i swiper
```
## Tailwind
> Then add Code050 UI to your `tailwind.config.js`
```tailwind.config.js
module.exports = {
darkMode: 'class',

    content: [
        './vendor/laravel/framework/src/Illuminate/Pagination/resources/views/*.blade.php',
        './vendor/laravel/jetstream/**/*.blade.php',
        './storage/framework/views/*.php',
        './resources/views/**/*.blade.php',
        "./node_modules/flowbite/**/*.js"
    ],

    theme: {
        extend: {
            fontFamily: {
                'headline': [
                    'Raleway', ...defaultTheme.fontFamily.sans
                ],
                'body': [
                    'nunito', defaultTheme.fontFamily.sans
                ],
                sans: [
                    'Nunito', ...defaultTheme.fontFamily.sans,
                ],
            },
            fontSize: {
                'display-lg': ['4rem', {
                    letterSpacing: '-.031rem',
                    lineHeight: '4.75rem'
                }],
                'display-md': ['3.563rem', {
                    letterSpacing: '-.016rem',
                    lineHeight: '4rem'
                }],
                'display-sm': ['2.813rem', {
                    letterSpacing: '0',
                    lineHeight: '3.25rem'
                }],

                'headline-lg': ['2rem', {
                    letterSpacing: '0',
                    lineHeight: '2.5rem'
                }],
                'headline-md': ['2rem', {
                    letterSpacing: '0',
                    lineHeight: '2.5rem'
                }],
                'headline-sm': ['2rem', {
                    letterSpacing: '0',
                    lineHeight: '2.5rem'
                }],

                'title-lg': ['1.375rem', {
                    letterSpacing: '0',
                    lineHeight: '2.5rem'
                }],
                'title-md': ['1rem', {
                    letterSpacing: '.006rem',
                    lineHeight: '1.5rem'
                }],
                'title-sm': ['.875rem', {
                    letterSpacing: '.006rem',
                    lineHeight: '1.25rem'
                }],

                'label-lg': ['.875rem', {
                    letterSpacing: '.006rem',
                    lineHeight: '1.25rem'
                }],
                'label-md': ['.75rem', {
                    letterSpacing: '.031rem',
                    lineHeight: '1rem'
                }],
                'label-sm': ['.688rem', {
                    letterSpacing: '.031rem',
                    lineHeight: '1rem'
                }],

                'body-lg': ['1rem', {
                    letterSpacing: '.031rem',
                    lineHeight: '1.5rem'
                }],
                'body-md': ['.875rem', {
                    letterSpacing: '.016rem',
                    lineHeight: '1.25rem'
                }],
                'body-sm': ['.75rem', {
                    letterSpacing: '.025rem',
                    lineHeight: '1rem'
                }],
            },
        },
    },
    daisyui: {
        themes: [
            {
                mytheme: {
                    "primary": "#17A660",
                    "secondary": "#6D97A3",
                    "accent": "#911BBA",
                    "neutral": "#454744",
                    "base-100": "#fff",
                    "base-200": "#efefef",
                    "base-300": "#E1E3DE",
                    "info": "#6D97A3",
                    "success": "#17A660",
                    "warning": "#FFAD40",
                    "error": "#FF5449",

                    "--rounded-box": "5px", // border radius rounded-box utility class, used in card and other large boxes
                    "--rounded-btn": "4px", // border radius rounded-btn utility class, used in buttons and similar element
                    "--rounded-badge": "1.9rem", // border radius rounded-badge utility class, used in badges and similar
                    "--animation-btn": "0.25s", // duration of animation when you click on button
                    "--animation-input": "0.2s", // duration of animation for inputs like checkbox, toggle, radio, etc
                    "--btn-text-case": "uppercase", // set default text transform for buttons
                    "--btn-focus-scale": "0.95", // scale transform of button when you focus on it
                    "--border-btn": "1px", // border width of buttons
                },
            }, 'luxury'

        ],
    },
    plugins: [
        require('@tailwindcss/forms'),
        require('@tailwindcss/typography'),
        require('daisyui'),
        require('flowbite/plugin')
    ],
```

---
<!-- ## Use
[See all components ->](https://www.documentatie.nl/components) -->

## Documents and examples
---
> See the official site: [code050-ui.com->](https://www.documentatie.nl/)
---
## List of components





* [Buttons](/components/actions/buttons.md)
* [Select](/components/actions/dropdown.md)
* [Cards](/Data-display/cards.md)
* [Team member block](/Data-display/team-member.md)
* [carousel](/Data-display/carousel.md)
* [Text input](/Data-input/input.md)
* [Text area](/components/actions/textarea.md)
* [Progress](/feedback/progress.md)
* [Dialog](/feedback/dialog.md)
* [Sections](/layouts/sections.md)
* [Footer](/layouts/footer.md)
* [Hero](/layouts/hero.md)
* [Divider](/layouts/divider.md)
* [Breadcrumbs](/Data-display/cards.md)
* [Link](/Data-display/cards.md)
* [Menu](/Data-display/cards.md)
* [Navbar](/Data-display/cards.md)