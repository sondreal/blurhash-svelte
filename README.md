# blurhash-svelte

![npm](https://img.shields.io/npm/v/blurhash-svelte)
![license](https://img.shields.io/npm/l/blurhash-svelte)
![issues](https://img.shields.io/github/issues/yourusername/blurhash-svelte)

`blurhash-svelte` is a Svelte component that decodes and displays BlurHash images. BlurHash is a compact representation of a placeholder for an image that can be displayed while the full image is loading.

## Features

- Simple and easy-to-use Svelte component
- Supports TypeScript with JSDoc annotations
- Highly customizable with width, height, and punch parameters

## Installation

To install the package, run:

```sh
npm install blurhash-svelte
```

## Usage
Here is a basic example of how to use the BlurHash component in your Svelte application:
```typescript
<script lang="ts">
  import BlurHash from 'blurhash-svelte/BlurHash.svelte';

  let hash = "LEHV6nWB2yk8pyo0adR*.7kCMdnj";
</script>

<BlurHash {hash} width={400} height={300} punch={1} />
```

## Props
The BlurHash component accepts the following props:
* `hash` (string): The BlurHash string.
* `width` (number, optional, default: 400): The width of the canvas.
* `height` (number, optional, default: 300): The height of the canvas.
* `punch` (number, optional, default: 1): The punch value for enhancing the contrast.

## Example 
```typescript
<script lang="ts">
  import BlurHash from 'blurhash-svelte/BlurHash.svelte';

  let hash = "LEHV6nWB2yk8pyo0adR*.7kCMdnj";
  let width = 500;
  let height = 350;
  let punch = 2;
</script>

<BlurHash {hash} {width} {height} {punch} />
```

## Development
To develop and build the package locally, follow these steps:
1. Clone the repository:
```sh
git clone https://github.com/sondreal/blurhash-svelte.git
cd blurhash-svelte
```
2. Install dependencies:
```sh
npm install
```
3. Start the development server:
```sh 
npm run dev
```
4. Build the package:
```sh
npm run build
```

## Contributing
Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
1. Create a new branch for your feature or bugfix.
1. Commit your changes.
1. Push the branch to your fork.
1. Create a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgements
* BlurHash by Wolt
* Svelte - The web framework for building high-performance web applications