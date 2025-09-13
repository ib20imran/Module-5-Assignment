# Module-5-Assignment
import 'dart:vmservice_io';

void main(){

  developer Developer = developer('md Imran ',102025,'Kasba',10250, 50000);
  Developer.displayInfo();
  Developer.Position();





}

class employer {

  String Companye = 'IB Studio';
  String ? Name ;
  //String ? Position  = 'Developer';
  int ? JoinDate;
  String ? Branch;

  employer( this.Name, this.JoinDate, this.Branch){

  }


  Position (){

    String position = 'java Developer';
    print(position);

  }

}

class developer extends employer {

  int ? id ;
  int? Salaye;

  developer (super.Name,super.JoinDate,super.Branch, this.id,this.Salaye);


  @override
  Position(){
     String position = 'Dart Developer';
     print("  " '$position');

  }


  displayInfo(){

  //print(developer(Name, '\n', JoinDate, Branch, id, Salaye));

    print( "  "'$Companye \n "ID=" $id \n "Name=" $Name \n "Join Date= " $JoinDate,'
        ' \n "Branch=" $Branch, \n "Salarye= " $Salaye,"TK" ');

  }




}
