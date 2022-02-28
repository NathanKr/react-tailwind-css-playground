<h2>Motivation</h2>
Setup for a react vite project with tailwind CSS

<h2>Installation</h2>
<h3>step 1</h3>
Terminal 
<ul>
<li>npm install -D tailwindcss postcss autoprefixer</li>
<li>npx tailwindcss init</li>
</ul>

The latter command has created tailwind.config.js
Edit it to have :
```

content: ["./index.html", "./src/**/*.{jsx,tsx,ts,js}"]

```


<h3>step 2</h3>
Add  the following file postcss.config.js
```

module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
};

```

<h3>step 3</h3>
Remove all content in index.css before adding 
@tailwind base;
@tailwind components;
@tailwind utilities;

<h3>step 4</h3>
Install vs. code plugin “PostCSS Language Support” (if not allready installed) to remove the warning in index.css

<h3>step 5</h3>
ovveride App.js :
```

export default function App() {
  return (
    h1 className="text-3xl font-bold underline text-center">
      Hello world Tailwind CSS!
    </h1>
  )
}

```

<h3>step 6</h3>
install dependencies from the terminal : 
npm i

<h2>Run the project</h2>
npm run dev
