# Kavita-tweaks

This repository includes some UI tweaks for [Kavita e-book server](https://github.com/Kareadita/Kavita).

## Installation

1. Move the CSS file to `config/themes/`
2. Activate in Settings
3. Enjoy!

![2022-05-27 22_23_08-Kavita - Dashboard](https://user-images.githubusercontent.com/1534150/170777564-452e2e7d-0bfe-4f92-a485-34182fc60c62.png)

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
