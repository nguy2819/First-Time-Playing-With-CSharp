# C#

- I built the HIGH-LOW GUESSING GAME SUCCESSFULLY - by MYSELF with some code helps for picking random number from my supervisor, David Borland.

```
namespace TienFirstFrameworkProject
{
    class GuessingGame
    {
        public static void Run()
        {
            Random rand = new Random();
            int number = rand.Next(1, 10);
            
            Console.Write("Enter a number from 1 to 10: ");

            while (true)
            {
                int num9 = Convert.ToInt32(Console.ReadLine());
                if (num9 > number)
                {
                    Console.WriteLine("Keep guessing! To HIGH!");
                    Console.Write("Guess again: ");
                } else if (num9 < number)
                {
                    Console.WriteLine("Keep guessing! To LOW!");
                    Console.Write("Guess again: ");
                } else
                {
                    Console.WriteLine("BINGO!");
                    break;
                }
            }
        }
    }
}
```