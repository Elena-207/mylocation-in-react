# React Geolocation App

This is a small React application that uses the browser's geolocation API to retrieve and display the user's GPS position. It also keeps track of how many times the user requests their position.

## How to Use

To use this application, follow these steps:

1. Clone the repository to your local machine.

```
git clone https://github.com/your-username/your-repository.git
```

2. Change into the project directory.

```
cd your-repository
```

3. Install the dependencies.

```
npm install
```

4. Start the development server.

```
npm start
```

The application will now be running at `http://localhost:3000`. Open this URL in your web browser to access the app.

## Features

- Click the "Get My Position" button to retrieve your GPS position.
- The application will display your latitude and longitude.
- It will also provide a link to view your location on OpenStreetMap.
- The number of times you request your position will be tracked and displayed on the screen.

## How it Works

The app is built using React and uses the `useState` hook to manage state. It contains a custom hook called `useGeolocation` that wraps the browser's geolocation API and handles retrieving the user's position and any errors that may occur.

The main component, `App`, renders a button to get the user's position. When the button is clicked, it increments the click counter and calls the `getPosition` function from the `useGeolocation` hook to get the GPS position.

If the geolocation is successful, it displays the latitude and longitude along with a link to OpenStreetMap. If there is an error (e.g., geolocation not supported or user denies permission), it displays the error message.

## Contributions

Contributions to this project are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

---

Happy geolocating! If you have any questions or need further assistance, feel free to reach out.
