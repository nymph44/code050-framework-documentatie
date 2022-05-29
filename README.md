# code050 UI
---
| Version  |1.0|
|---------|------------|
| Total Components | 18 |
| License | Alexander Janssen|
| Last commit | May 29 2022|

[Official website](https://www.code050.nl)

[Components](https://www.code050.nl)

[How to use](https://www.code050.nl)

---
## Features
* Consistency inside the Code050 ecosystem
* Cleaner code
* Reusability

---
## Install now!
    git clone https://github.com/nymph44/code050-framework-documentatie.git

> In order to to fully use the framework you need to install Daisy UI and Flowbite to make use of the required plugins.

    npm i Daisyui

> and

    npm i flowbite

> Then add Code050 UI to your `tailwind.config.js`

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

            gradients: {
                'darkoverlay': "linear-gradient(0deg, rgba(2,0,36,1) 0%, rgba(0,0,0,1) 44%, rgba(0,0,0,0) 100%);",
            },
            colors: {
                transparent: 'transparent',
                'forest': {
                    'DEFAULT': '#00894A',
                    990: '#00210D',
                    950: '#00391B',
                    900: '#00522A',
                    800: '#006D3A',
                    700: '#00894A',
                    600: '#17A660',
                    500: '#40C178',
                    400: '#60DE92',
                    300: '#7EFBAC',
                    200: '#C1FFD3',
                    100: '#F3FFF3',
                },
                'stone': {
                    'DEFAULT': '#757874',
                    990: '#1A1C1A',
                    950: '#2E312E',
                    900: '#454744',
                    800: '#5C5F5B',
                    700: '#757874',
                    600: '#8F918D',
                    500: '#A9ACA7',
                    400: '#C6C7C3',
                    300: '#E1E3DE',
                    200: '#F0F1EC',
                    100: '#FBFDF7',
                },
            },
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

[Read more](https://www.code050.nl)
---
## Use
[See all components ->](https://www.documentatie.nl/components)

## Documents and examples
---
> See the official site: [code050-ui.com->](https://www.documentatie.nl/)
---
## List of components



* [Buttons](/components/actions/buttons.md)
* [Dropdown](/components/actions/dropdown.md)
* [Modal](/components/actions/modal.md)