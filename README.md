# YAML | YML Example

## __***Yaml example***__

```yaml
person:
  name: &name "Eddy"(:33)
  ocuppation: "Developer"
  age: 24
  size: !!float 2
  gpa: 3.5
  volume: !!str 40.4
  fav_num: 1e+10
  male: true
  birthday: 1996-02-08
  flaws: null
  hobbies:
    - hiking
    - movies
    - riding bike
  movies: ["Dark Knight", "Good Will Hounting"]
  friends:
    - name: "Steph"
      age: 22
    - {name: "Adam", age: 22}
    -
      name: "joe"
      age: 23
  description: >
    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, 
    when an unknown printer took a galley of type and scrambled it to make a typ
  signature: |
    Mike
    Giraffe Acatemy
    Email...
  id: *name

  base: &base
    var1: value1
    var2: 22
  
  foo:
    <<: *base
    var3: something else
```
## __***JSON example***__

```json
{
    "person": {
        "name": "Eddy",
        "ocuppation": "Developer",
        "age": 24,
        "size": 2,
        "gpa": 3.5,
        "volume": "40.4",
        "fav_num": 10000000000,
        "male": true,
        "birthday": "1996-02-08T00:00:00.000Z",
        "flaws": null,
        "hobbies": ["hiking", "movies", "riding bike"],
        "movies": ["Dark Knight", "Good Will Hounting"],
        "friends": [
            {
                "name": "Steph",
                "age": 22
            },
            {
                "name": "Adam",
                "age": 22
            },
            {
                "name": "joe",
                "age": 23
            }
        ],
        "description": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,  when an unknown printer took a galley of type and scrambled it to make a typ\n",
        "signature": "Mike\nGiraffe Acatemy\nEmail...\n",
        "id": "Eddy",
        "base": {
            "var1": "value1",
            "var2": 22
        },
        "foo": {
            "var1": "value1",
            "var2": 22,
            "var3": "something else"
        }
    }
}

```