# code_style
Code styles, and tools for different languages

# General conventions

- Clients should send the next headers on every request to our api:

  * `bv-app-version`: `platform/typeApp/version/build` (**each value separated by `/`**) where:

    - `platform`: platform who make the request in lower case (ej: ios, android)
    - `typeApp`: app profile who make the request in lower case (ej: customer, driver, admin) if there are only one app could be mobile for mobile apps
    - `version`: current app version following semver standard (x.y.z)
    - `build` **(optional)** : current build version, could be number or letters
