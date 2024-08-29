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
   
   CACHORRO QUENTE
   PAO NA CHAPA 
   
   BIFE A PAULISTA 
   CHURRASCO 
   
   pudim 
   brigadeiro 
   
   
			), //Padding
		), //SizedBox
);}

