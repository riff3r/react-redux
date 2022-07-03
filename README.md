# Redux

## index.js boilerplate

import React from "react";
import { ReactDOM } from "react";
import { Provider } from "react-redux";
import { createStore } from "redux";
import reducers from "./reducers";

import App from "./App";

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(
<Provider store={createStore(reducers)}>
<React.StrictMode>
<App />
</React.StrictMode>
</Provider>
);
