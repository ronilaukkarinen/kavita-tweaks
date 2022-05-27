# Kavita-tweaks

This repository includes some UI tweaks for [Kavita e-book server](https://github.com/Kareadita/Kavita).

## Installation

1. Move the CSS file to `config/themes/`
2. Activate in Settings
3. Enjoy!

## Progress of the book

1. Get [Custom JavaScript for Websites](https://chrome.google.com/webstore/detail/custom-javascript-for-web/ddbjnfjiigjmcpcpkmhogomapikjbjdk).
2. Add following script:

```js
const progresses = document.querySelectorAll('.progress');

progresses.forEach((progress) => {
  const progressBar = progress.querySelector('.progress-bar');
  const percentageAmount = parseInt(progressBar.offsetWidth);

  console.log(progressBar);
  progress.insertAdjacentHTML('afterend', '<div class="percentage bg-primary">' + percentageAmount + '%</div>');
});
```
