# DCIT-318--Assignment-10823856 ( price calculator) 



using System;

namespace TicketPriceCalculator
{
    class Program
    {
        static void Main(string[] args)
        {
            //  regular and discount ticket prices
            decimal regularPrice = 10.0m;
            decimal discountPrice = 7.0m;

            // Prompt the user to enter the age of the customer
            Console.Write("Enter the age of the customer: ");
            int age = int.Parse(Console.ReadLine());

            // ticket price based on the age of the customer
            decimal ticketPrice;
            if (age <= 12 || age >= 65)
            {
                ticketPrice = discountPrice;
            }
            else
            {
                ticketPrice = regularPrice;
            }

            // the ticket price
            Console.WriteLine("The ticket price is: GHC" + ticketPrice);
        }
    }
}
