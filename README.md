# Image Inpainting Widget

This is an image inpainting tool built with React and `react-canvas-draw`. It allows users to upload an image, draw over it to mask specific areas, and export the generated mask.

## Features
- Upload an image to inpaint.
- Draw on the image with adjustable brush size.
- Export the mask as a PNG image.

## How to Run the Project Locally

### Prerequisites
- **Node.js** (v16 or higher)
- **npm** 

### Steps

1. Clone the repository to your local machine:
   in CMD run following command:
   git clone <https://github.com/jharianeetu/React_Asssignment>
   
   navigate to project folder:
   cd image-inpainting-widget

2.Install the dependencies:

	in cmd run following command:
	npm install
	
3.Start the development server:


	run following command to run:
	npm run dev
	
	
### Libraries Used:
1. React: A JavaScript library for building user interfaces.
   Version: ^17.0.2

2. react-canvas-draw: A React component for drawing on a canvas, used for inpainting functionality.
   Version: ^1.2.1

3.@eslint/js: ESLint configuration for JavaScript code.
  Version: ^9.15.0

4. @types/react: TypeScript type definitions for React.
   Version: ^18.3.12
   
5. @types/react-dom: TypeScript type definitions for React DOM.
  Version: ^18.3.1
  
6. @vitejs/plugin-react: Vite plugin for React, helps in fast React development with Vite.
   Version: ^4.3.4

7. eslint-plugin-react: ESLint plugin for React-specific linting rules.
   Version: ^7.37.2
   
8. eslint-plugin-react-hooks: ESLint plugin for React Hooks linting.
   Version: ^5.0.0
   
9. eslint-plugin-react-refresh: Plugin for linting React Fast Refresh.
   Version: ^0.4.14
   
10. globals: Provides global variables for various environments to avoid ESLint errors.
    Version: ^15.12.0
	
11. vite: A next-generation, fast build tool and development server.
    Version: ^6.0.1

### Challenges Faced and Solutions:
1.Canvas Handling: Used react-canvas-draw to manage drawing and erasing on the canvas, adjusting brush size dynamically.
2.Image Upload: Utilized <input type="file"> and URL.createObjectURL() to handle image uploads and render them.
3.Mask Generation: Created a separate mask canvas to export a black-and-white mask using toDataURL() for download.
4.UI Consistency: Ensured responsive and consistent styling using CSS and flexbox for layout adjustments.
5.Performance: Optimized by using useRef and useEffect to minimize unnecessary re-renders and improve responsiveness.
6.Cross-Browser Compatibility: Tested and ensured functionality across multiple browsers by using standard HTML5 APIs.
7.Download Feature: Implemented automatic mask image download using a temporary <a> element with the download attribute.
8.Brush Size Control: Adjusted brush size interactively with a slider, ensuring smooth updates on the canvas.
9.Canvas Size: Set fixed canvas dimensions but allowed adjustments for different image sizes.
10.Real-Time Updates: Used React's state and effect hooks to update the mask in real-time as the user drew on the canvas.
