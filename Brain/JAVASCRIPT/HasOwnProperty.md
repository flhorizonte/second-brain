### HasOwnProperty

- Verifica se a propriedade do objeto existe.

- Existe dois tipos de propriedades: Propriedades próprias e propriedades prototipadas.
	
		if(duck.hasOwnProperty(property)) {
			    ownProps.push(property); //own
		  } else {
			    prototypeProps.push(property);  //prototype
		  }