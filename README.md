# Web3-React-Native

* Use Expo for installing and starting the project.

## Basics

1. View is like div in comparison
2. Text is like p in comparison
3. The elements should be wrapped inside a <View> tag.
4. StyleSheet is used for styling components
5. The styles key should be camelCase
6. The styles value should be inside inverted commas  

```
Basic anaotmy of the file

// Imports

// Function

// Styles

// Export

```

## React Navigation

React navigation is used for navigating between comnponents/screens. 

### Steps

1. Create a folder -> src -> components
2. Create a custom component -> First.js
3. Install required dependencies
4. Import the dependencies  
5. Go to App.js and wrap everything in NavigationContainer  
  
## Lists  
  
```
  
<Import code here>

const First = () => {

    const data = [1,2,3,4];


  return (
    <View style={styles.container}>

        {data.map((value,index)=>{
            return(

                <Text style={styles.textStyle}>{value}</Text>

            )
        })}

      
      
    </View>
  );
}

const styles = <Styles code here>

export default First;

  ```

The above code is same as in normal React. But, for React-native we have FlatList.
  
```
  
<import code>

const First = () => {

    const data = [1,2,3,4];


  return (
    <View style={styles.container}>

        {data.map((value,index)=>{
            return(

                <Text style={styles.textStyle}>{value}</Text>

            )
        })}


        <FlatList
        data={data}
         renderItem = {({item,index})=>{

            return(
                <Text key={index} style={styles.textStyle}>{item}</Text>
            )

        }}
        />

      
      
    </View>
  );
}

<style code>

export default First;

```
  
## Navigation
  
1. Button component is a simple component for showing button and detecting a press
2. TouchableOpacity is a custom component which can detect any type of press on it
3. 
  
  ```
  
// Imports

const First = ({ navigation }) => {

    const data = [1,2,3,4];


  return (
    <View style={styles.container}>

            <Button
                title="Go to Main"
                onPress={() => navigation.navigate('Home')}
            />

        <FlatList
        data={data}

        renderItem = {({item,index})=>{

            return(
                <Text key={index} style={styles.textStyle}>{item}</Text>
            )

        }}
        />

      
      
    </View>
  );
}

// Styles

export default First;

              ```
              
## State Management
              
              


## Official Docs
1. React native docs : https://reactnative.dev/
2. Expo docs : https://docs.expo.dev/workflow/expo-cli/
3. React-native navigation: https://reactnavigation.org/  
