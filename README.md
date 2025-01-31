Here is a `README.md` file for your React application:

```markdown
# React Background Color Changer

This is a simple React application that allows users to change the background color of the screen by clicking on different buttons.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/your-username/react-background-color-changer.git
   cd react-background-color-changer
   ```

2. **Install dependencies:**

   ```sh
   npm install
   ```

3. **Start the development server:**

   ```sh
   npm run dev
   ```

## Usage

Open your browser and navigate to `http://localhost:3000`. You will see a screen with buttons to change the background color.

## Code Explanation

The main functionality is within the `App` component:

```jsx
import { useState } from 'react'
import reactLogo from './assets/react.svg'
import viteLogo from '/vite.svg'
import './App.css'

function App() {
  const [color, setColor] = useState("yellow")

  return (
    <div className='flex flex-wrap justify-center w-screen h-screen p-0' style={{ backgroundColor: color }}>
      <div className='bottom-8 w-80 mt-72 bg-white border-2 border-black h-10 rounded-lg flex gap-5 ml-3 flex-row pl-5'>
        <button className='bg-red-600 border-2 border-black rounded-md h-9 w-20' 
          onClick={() => setColor("red")}>
          Red
        </button>
        <button className='bg-blue-600 border-2 border-black rounded-md h-9 w-20' 
          onClick={() => setColor("blue")}>
          Blue
        </button>
        <button className='bg-green-600 border-2 border-black rounded-md h-9 w-20' 
          onClick={() => setColor("green")}>
          Green
        </button>
      </div>
    </div>
  )
}

export default App
```

### Explanation:

- **State Management:**
  - The `color` state is initialized with a default value of `"yellow"`.
  - The `setColor` function is used to update the background color.

- **JSX Structure:**
  - A `div` is styled to take up the entire viewport (`w-screen h-screen`).
  - The `style` prop is used to dynamically set the background color based on the `color` state.
  - A container `div` holds three buttons, each with an `onClick` event handler to change the background color.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

This `README.md` provides an overview of the project, installation instructions, usage details, a brief code explanation, and sections for contributing and the license.
