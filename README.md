# clasemovil111


import { StatusBar } from 'expo-status-bar';
import React from 'react';
import { Button, StyleSheet, Text, View, Button, Alert } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <Text>Open up App.js to start working on your app!</Text>
      <StatusBar style="auto" />
      <View>
        <Text style={[style.AzulGrande, style.ColorRojo]}>
          Formatos
        </Text>
      </View>
      <View>
        <Button title="Precionar"
        onPress={()=>Alert.alert('Preciono el BOoton')}>
          <View>
            <TextInput>

            </TextInput>
          </View>
        </Button>
      </View>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
    backgroundColor: "orange",
  },
  AzulGrande:{
    color:'blue',
    fontWeight: 'bold',
    fontSize: 30,
  },
  ColorRojo:{
   color: 'red',
  },
  TextoInpo:{
    underLineColorAndroid:"transparent",
    placeholder:"Email",
    onChangeText:this.handleEmail,
  },
  datoNymerico:{

  },
  Alfanumerico:{

  },
  Passwordc:{
    underLineColorAndroid:"transparent",
    placeholder:"Clave",
    placeholderTevtColor:"blue",
    onChangeText:this.handlePassword,
  },

});
