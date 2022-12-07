import { StatusBar } from 'expo-status-bar';
import React, { useState } from 'react';
import { StyleSheet, Text, View, Button, createElement, Image, SafeAreaView, TouchableOpacity } from 'react-native';
 
 
export default function App() {
  const [textoInicial, setTextoInicial,] = useState("");
  
  
  return (
    
    
    
    <View style={styles.container}>
      
  <Text style ={{color:"Black", 
    fontSize: 80, 
    margin: 20,}}>
     GABI    
     </Text>

    <TouchableOpacity>
  style= {styles.buttongabi}
    <Image>
      source=  {require('./assets/Fotogabi.png')}
      style= {styles.fotobuttongabi}
    </Image>
    </TouchableOpacity>




     <Button title = 'Next'
     style={styles.tecla}/>
     <Image source={require('./assets/Fotogabi.png')}
     style={styles.logo}/>
    <StatusBar style="auto" />
      




    </View>
  );
 
 
}
 
const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: 'white',
    alignItems: 'center',
    justifyContent: 'center',

  },

  logo:{
    alignItems:"stretch"
  }
  
  ,
  tecla:{
  alignItems:"flex-end"
  
  }
  
});

 
