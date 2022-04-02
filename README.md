# Mutex-2-roblox-instance-
Open 2 roblox instances
Note: run on admin or it wont work
script: using System;
using System.Runtime.InteropServices;
using System.Threading;

namespace ConsoleApp2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Press A to enable 2 roblox instance feature");
            while (true)
                if (Console.KeyAvailable)
                    if (Console.ReadKey(true).Key == ConsoleKey.A)
                    {

                        Console.ForegroundColor = ConsoleColor.DarkMagenta;
                        Console.WriteLine("Pressed A!");
                        Console.WriteLine("Closing handle BaseNamedObjects ROBLOX singletonEvent");
                        Console.WriteLine("Closing handle......");
                        Console.WriteLine("Closed handle successfully");
                        Console.WriteLine("Join our discord https://discord.gg/kY5JyPQ3HZ");
                        Console.WriteLine("Note: Please do not close out of this");
                        Console.WriteLine("Thank you so much for using this app! We hope to see you again on our site!");
                        Console.Title = "Multiple Roblox Instances";
                        Console.ForegroundColor = ConsoleColor.Red;
                        new Mutex(true, "ROBLOX_singletonMutex");
                        Console.Write("Multiple Roblox Instances is now running!\n");
                        Console.ReadLine();


                    }

        }
    }
}


main part of script:
                        new Mutex(true, "ROBLOX_singletonMutex");
                        Console.Write("Multiple Roblox Instances is now running!\n");
                        Console.ReadLine();
