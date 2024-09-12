# cc


import 'package:flutter/material.dart';
// ignore: unnecessary_import
import 'dart:ui';
//imported google's material design library
void main() {
// ignore: unnecessary_const
const circleAvatar = const CircleAvatar(
			 backgroundImage: AssetImage('assets/coxinha.jpg'),
					radius: 100,
					);
runApp(
	/**Our App Widget Tree Starts Here**/
	MaterialApp(
	home: Scaffold(
	appBar: AppBar(
	), //AppBar
	body: Center(
		/** Card Widget **/
		child: Card(
		elevation: 50,
		shadowColor: Colors.black,
		color: Colors.greenAccent[100],
		child: SizedBox(
			width: 300,
			height: 450,
			child: Padding(
			padding: const EdgeInsets.all(20.0),
			child: Column(
				children: [
				CircleAvatar(
					backgroundColor: Colors.green[500],
					radius: 108,
					child: circleAvatar, //CircleAvatar
				), //CircleAvatar
				const SizedBox(
					height: 10,
				), //SizedBox
				Text(
					'Coxinha',
					style: TextStyle(
					fontSize: 30,
					color: Colors.green[900],
					fontWeight: FontWeight.w500,
					), //Textstyle
				), //Text
				const SizedBox(
					height: 10,
				), //SizedBox
				
						],
						),
					),
					),
					// RaisedButton is deprecated and should not be used
					// Use ElevatedButton instead

					// child: RaisedButton(
					// onPressed: () => null,
					// color: Colors.green,
					// child: Padding(
					//	 padding: const EdgeInsets.all(4.0),
					//	 child: Row(
					//	 children: const [
					//		 Icon(Icons.touch_app),
					//		 Text('Visit'),
					//	 ],
					//	 ), //Row
					// ), //Padding
					// ), //RaisedButton
				) //SizedBox
				
			), //Column


			), //Padding
		), //SizedBox
);}




   // 
   COXINHA
   FEIJOADA 
   
   PAO COM MORTADELA 
   PASTEL 
   
   Hamburguer 
   PAO NA CHAPA 
   
   BIFE A PAULISTA 
   CHURRASCO 
   
   pudim 
   brigadeiro 
   
   
			), //Padding
		), //SizedBox
);}

-------------------------------------



--------------------------

import 'package:flutter/material.dart';

void main() {
  runApp(
    MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text('Card Example'),
        ),
        body: GridView.builder(
          gridDelegate: const SliverGridDelegateWithFixedCrossAxisCount(
            crossAxisCount: 2, // Número de colunas
            crossAxisSpacing: 10.0, // Espaçamento horizontal entre colunas
            mainAxisSpacing: 10.0, // Espaçamento vertical entre linhas
          ),
          padding: const EdgeInsets.all(10.0),
          itemCount: 8, // Número total de cards
          itemBuilder: (context, index) {
            // Lista de caminhos de imagens
            final List<String> images = [
              'assets/coxinha.jpg',
              'assets/bife.jpg',
              'assets/pao.jpg',
              'assets/chapa.jpg',
              'assets/queijo.jpg',
              'assets/churrasco.jpg',
              'assets/brigadeiro.jpg',
              'assets/lasanha.jpg',
            ];

            // Obtém a imagem correspondente ao índice
            final String imagePath = images[index % images.length];

            return Card(
              shadowColor: Colors.black,
              color: const Color.fromARGB(255, 41, 41, 41),
              child: SizedBox(
                width: 150, // Largura do card
                height: 180, // Altura do card
                child: Padding(
                  padding: const EdgeInsets.all(20.0),
                  child: Column(
                    children: [
                      CircleAvatar(
                        backgroundImage: AssetImage(imagePath),
                        radius: 50,
                      ),
                      const SizedBox(height: 10),
                      const Text(
                        'Coxinha',
                        style: TextStyle(
                          fontSize: 20,
                          color: Colors.white,
                          fontWeight: FontWeight.w500,
                        ),
                      ),
                      const SizedBox(height: 10),
                      ElevatedButton(
                        onPressed: () {}, // Placeholder action
                        style: ElevatedButton.styleFrom(
                          backgroundColor: const Color.fromARGB(255, 105, 103, 103), // Button background color
                        ),
                        child: const Padding(
                          padding: EdgeInsets.all(4.0),
                          child: Row(
                            mainAxisSize: MainAxisSize.min,
                            children: [
                              Text(
                                'Ver Mais',
                                style: TextStyle(
                                  color: Color.fromARGB(255, 255, 255, 255), // Text color
                                ),
                              ),
                            ],
                          ),
                        ),
                      ),
                    ],
                  ),
                ),
              ),
            );
          },
        ),
      ),
    ),
  );
}



// funcionou - colocar nome e lins da pag

