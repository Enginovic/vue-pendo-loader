# Vue Pendo Loader

This project is a Vue.js plugin for integrating Pendo into your Vue applications. Pendo helps you understand and guide your users to create product experiences they love.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Installation

To install the Vue Pendo Loader, you can use npm or yarn:

```bash
npm install vue-pendo-loader
```

or

```bash
yarn add vue-pendo-loader
```

## Usage

First, import and use the plugin in your Vue application:

```javascript
import Vue from 'vue';
import VuePendoLoader from 'vue-pendo-loader';

Vue.use(VuePendoLoader, {
	apiKey: 'YOUR_PENDO_API_KEY',
});
```

Then, you can use Pendo in your components:

```javascript
export default {
	name: 'YourComponent',
	mounted() {
		this.$pendo.initialize();
	},
};
```

## Configuration

You need to provide your Pendo API key when initializing the plugin. You can also pass additional configuration options as needed.

```javascript
Vue.use(VuePendoLoader, {
	apiKey: 'YOUR_PENDO_API_KEY',
	additionalOption: 'value',
});
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any bugs or feature requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
