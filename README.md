# Immutable Persistence Transform

## Why?

## Installation

## How to use?

```javascript
import { createStore } from "redux";
import { persistStore, persistReducer } from "redux-persist";
import storage from "redux-persist/lib/storage";

import ImmutablePersistenceTransform from "redux-immutable-persistence-transform";
import reducers from "./ducks";

const persistConfig = {
  key: "root",
  storage,
  transforms: [ImmutablePersistenceTansform]
};

const persistedReducer = persistReducer(persistConfig, reducers);

const store = createStore(persistedReducer);
const persistor = persistStore(store);

export { store, persistor };
```

## Contribution

## License

Distributed under the MIT license. See LICENSE for more information.

## Contact

Gleydson Rodrigues - [Github](https://github.com/gleydson) - **gleydsonsr@gmail.com**
