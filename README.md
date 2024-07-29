using DocumentFormat.OpenXml.Office2013.Word;
using System;
using System.Collections.Generic;
using System.Linq;
using System.Reflection.Metadata.Ecma335;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp8
{
    class Program
    {


        static void Main(string[] args)


        {


            {
                car car1 = new car();
                car1.carname = "peykan";
                car1.carspeed = "20000";
                car1.carmodel = "96";

                car car2 = new car();
                car2.carname = "pride";
                car2.carspeed = "100";
                car2.carmodel = "1400 \n ";

                Console.WriteLine(car1.carname + " " + car1.carspeed + " " + car1.carmodel);
                Console.WriteLine(car2.carname + " " + car2.carspeed + " " + car2.carmodel);



                person person1 = new person("yara", "nourkhani", "20");
                person person2 = new person("moein", "heydari", "20");


                Console.WriteLine($" name : {person1.name} \n familyname : {person1.familyname}  \n age : {person1.age} \n ");

                Console.WriteLine($" name : {person2.name}  \n familyname : {person2.familyname} \n  age : {person2.age}");

                Console.ForegroundColor = ConsoleColor.Green;

                Console.WriteLine("**********************");

                Console.ResetColor();

                Console.WriteLine("please enter your number:");

                int number = Convert.ToInt32(Console.ReadLine());
                person[] people = new person[number];

                for (int i = 0; i < number; i++) ;

                Console.ForegroundColor = ConsoleColor.Green;

                Console.WriteLine("**********************");

                Console.ResetColor();

             
            }
        }
    }
}

    internal class car    {
        public string carname;        public string carspeed;
        public string carmodel;
    }}







    internal class personBase
    {
        public string name;
        public string familyname;
        public string age;

        public personBase()
        {
        }

        public personBase(string name, string familyname, string age)

        {
            this.name = name;
            this.familyname = familyname;
            this.age = age;

        }
    }
}

