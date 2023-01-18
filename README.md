# Boolder Data

[Boolder](https://www.boolder.com) is the best way to discover bouldering in Fontainebleau.

Here is the data used by the [Android](https://github.com/boolder-org/boolder-android) and iPhone apps. Feel free to use it as you want!

## License

[![Creative Commons License](https://i.creativecommons.org/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)  

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

## Database

The `boolder.db` file is an [SQLite](https://en.wikipedia.org/wiki/SQLite) database with the following tables:

### problems

| Column          | Type      | Example             | Description   |
| --------------- | --------- | -------------       | ------------- |
| id              | `INTEGER` | 506                 | Boolder id    |
| name            | `STRING`  | La Marie-Rose       | Name of the problem |
| grade           | `STRING`  | 6a                  | [Fontainebleau-style grade](https://en.wikipedia.org/wiki/Grade_(bouldering)#Fontainebleau_grades) from 1a to 9c+ |
| latitude        | `REAL`    | 48.44706625262      | GPS latitude |
| longitude       | `REAL`    | 2.63909882977       | GPS longitude |
| circuit_id      | `INTEGER` | 15                  | used to join on circuits table |
| circuit_number  | `TEXT`    | 22                  | number within the circuit |
| circuit_color   | `TEXT`    | red                 | possible values: yellow purple orange green blue skyblue salmon red black white |
| steepness       | `TEXT`    | wall                | possible values: wall slab overhang roof traverse other |
| sit_start       | `INTEGER` | 1                   | `1` for sit start, `0` for normal start  |
| area_id         | `INTEGER` | 4                   | used to join on areas table |
| bleau_info_id   | `INTEGER` | 2128                | Id on bleau.info |
| featured        | `INTEGER` | 1                   | `1` if problem is "popular", `0` otherwise |
| popularity      | `INTEGER` | 14923               | the higher the more popular |
| parent_id       | `INTEGER` | 1234                | id of the parent problem (if it exists) |

### areas

Todo

### circuits

Todo

### lines

Todo

### pois

Todo

### poi_routes

Todo

## Geojson files

Todo

Recommended tool to view/edit geojson files: [JOSM](https://josm.openstreetmap.de)

<img width="1621" alt="JOSM screenshot" src="https://user-images.githubusercontent.com/330823/213291501-3c9f50c4-a65e-41eb-9099-6e84e5c2e3b0.png">


## Topo photos (beta)

Todo
