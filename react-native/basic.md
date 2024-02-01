## A. Instalasi React Native

## B. Basic

1. Views and Mobile Development

View adalah tampilan utama dalam mobile React Native.

2. Navtive Components

React Native memiliki compnents yang sudah disediakan (Natiive Components). Selain itu kita bisa membuat components native kita sendiri

3. Core Components

Core Components adalah Api components yang disediakan oleh React Native. Salah satu Core Components: View, Text, Image, ScrollView, TextInput, dll.

**Kesimpulan**: Jadi React Compnents itu terdiri dari React Native Components yang mana terdiri dari 3 bagian yaitu: Community Components, Core Components,Your Native Components.

## C. React Fundamentals

React Native berjalan di React. Beberapa konspe dalam React antara lain:

- Compnents

Components yaitu sebuah blueprint.

```Javascript
import React from "react";
import {Text} from "react-nativ";

const Cat = () => {
  return <Text>Ini adalah compnents</Text>
}

export default Cat;
```

- JSX

JSX adalah sintak yang dapat didalamnya terdapat element.

```Javascript
import React from "react";
import {Text} from "react-native";

const getFullName = (fname, mname, lname,) =>{
  return fname + " " + mname + " " + lname;
}

const Cat = () => {
  return <Text>Hello, I am {getFullName("asraf", "takayuma", "ganteng")}</Text>
}

export default Cat;

```

Terdapat juga Custom Components yaitu Component yang dibuat sendiri. Selain itu jika terdapat komponent yang dirender oleh component lain maka dia menjadi component anak dan yang yang merender adalah komponent parent.

```Javascript
{/* Child Compnents */}
const Cat = () => {
  return <Text>Ini adalah compnents</Text>
}

{/* Parent Compnents */}
const Cafe = () => {
  return (
    <View>
      <Cat />
      <Cat />
      <Cat />
    </View>
  )
}
```

- Props

Props adalah singkatan dari "properties" hal ini hampir mirip dengan parameter.

```Javascript
const Cat = (props) => {
  return <Text>Ini adalah compnents {props.name}</Text>
}


const Cafe = () => {
  return (
    <View>
      <Cat name="yums" />
      <Cat name="kitty" />
    </View>
  )
}

export default Cafe;
```

- State

State digunakan untuk pengolahan data yang berubah dalam React.

```Javascript
import React, {useState} from 'react';
import {Button, Text, View} from 'react-native';

const Cat = props => {
  const [isHungry, setIsHungry] = useState(true); // State

  return (
    <View>
      <Text>
        I am {props.name}, and I am {isHungry ? 'hungry' : 'full'}!
      </Text>
      <Button
        onPress={() => {
          setIsHungry(false);
        }}
        disabled={!isHungry}
        title={isHungry ? 'Pour me some milk, please!' : 'Thank you!'}
      />
    </View>
  );
};

const Cafe = () => {
  return (
    <>
      <Cat name="Munkustrap" />
      <Cat name="Spot" />
    </>
  );
};
```
