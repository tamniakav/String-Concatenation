# String-Concatenation
Just another repository
using System;

namespace _11.String_Concatenation
{
    class Program
    {
        static void Main(string[] args)
        {
            char simbol = char.Parse(Console.ReadLine());
            string evenOrOdd = Console.ReadLine();
            int n = int.Parse(Console.ReadLine());

            string words = string.Empty;

            for (int i = 1; i <= n; i++)
            {
                int num = i % 2;
                string word = Console.ReadLine();

                if (evenOrOdd == "even")
                {
                    if (num == 0)
                    {
                        words += word;                  
                        words += simbol;
                    }
                }
                else
                {
                    if (num == 1)
                    {
                        words += word;                      
                        words += simbol;
                    }
                }
            }          

            words = words.Remove(words.Length - 1);

            Console.WriteLine(words);
        }
    }
}
