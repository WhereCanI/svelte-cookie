<br/>
<p align="center">
  <h3 align="center">Svelte-Cookie</h3>

  <p align="center">
    A tool that will make setting, getting and deleting cookie's easier in your Svelte project.
    <br/>
    <br/>
    <a href="https://github.com/WhereCanI/Svelte-Cookie/issues">Report Bug</a>
    .
    <a href="https://github.com/WhereCanI/Svelte-Cookie/issues">Request Feature</a>
  </p>
</p>

![Downloads](https://img.shields.io/github/downloads/WhereCanI/Svelte-Cookie/total) ![Contributors](https://img.shields.io/github/contributors/WhereCanI/Svelte-Cookie?color=dark-green) ![Issues](https://img.shields.io/github/issues/WhereCanI/Svelte-Cookie) ![License](https://img.shields.io/github/license/WhereCanI/Svelte-Cookie) 

## Table Of Contents

* [About the Project](#about-the-project)
* [Getting Started](#getting-started)
  * [Installation](#installation)
* [Usage](#usage)
* [License](#license)
* [Authors](#authors)
* [Acknowledgements](#acknowledgements)

## About The Project

Cookies are very often used in today's websites and web applications, but handling cookies in plain Javascript can be complicated. With Svelte-Cookie the complicated and complex cookie handling is over.

Here's why:

* With the getCookie function, you can quickly get a cookie from the browser.
* With the setCookie function, you can easily create a new cookie that will be set in the web browser.
* With the deleteCookie function, you can quickly erase an existing cookie from the web browser.

## Getting Started

It's very easy to get started with Svelte-Cookie. Follow the instructions below, and you will be working with cookies in no time.

### Installation

To install, please write the following in your terminal:
```sh
npm install --save svelte-cookie
```

## Usage

To use svelte-cookie, please start by importing the desired functions to your project. As of this moment, svelte-cookie contains 3 functions which are:
* getCookie
* setCookie
* deleteCookie

You can import them by using the following line:
```sh
import { getCookie, setCookie, deleteCookie } from 'svelte-cookie';
```

## Examples
Underneath here you will find some examples of ways to use the individual functions:

**getCookie:**
The getCookie function is as the name says, getting a cookie. You do that by providing the name of the cookie. If the cookie exists the value length will be longer than 0.

```
let co = getCookie('userEmail');
```
If the userEmail cookie exist, you will get back the value. If it doesn't exist you will get back an empty string.

**setCookie:**
The setCookie allows you to add a cookie to the web browser in only a few steps. The setCookie has some options which you have to provide:

* Name - The first parameter is the name of the cookie.
* Value - The second parameter is the string value you want to cookie to have.
* Expiration days - Provide a number of how many days your cookie should stay in the web browser.
* Secure - Write either true or false depending on whether you want your cookie to have the secure attribute.

```
setCookie('userEmail', 'example-name@example.com', 30, true);
```

The above code will create a cookie named "userEmail", with the value "example-name@example.com". It will expire in 30 days and it will be set as secure.

**deleteCookie:**
The deleteCookie function is very simple, and it will allow you to quickly erase a cookie from the web browser. You simply provide the name of the cookie as shown in the example below:

```
deleteCookie('userEmail');
```

## License

Distributed under the MIT License. See [LICENSE](https://github.com/WhereCanI/Svelte-Cookie/blob/main/LICENSE.md) for more information.

## Authors

* **Michael Andersen** - *Frontend web developer* - [Michael Andersen](https://github.com/WhereCanI/) - *Built Svelte-Cookie*

[SustainableWWW](https://sustainablewww.org) - Learn about environmentally friendly and ethical web design.