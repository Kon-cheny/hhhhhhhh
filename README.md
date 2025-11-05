using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace dll.l
{
    public class Instrument_1
    {
        /// <summary>
        /// Функция выводит приветствие 
        /// </summary>
        /// <param name="name"></param>
        public void HelloWorld(string name)
        {
            Console.WriteLine($"Привет, {name}");
        }
        /// <summary>
        /// Функция считает возвраст пользователя через 5 лет
        /// </summary>
        /// <param name="age"></param>
        /// <returns></returns>
        public int AgeToFive(int age) 
        { 
            return age + 5;
        }

    }
}





using System.Diagnostics.Metrics;
using dll.l;

public class Instrument
{
    static void Main(string[] age)
    {
        Instrument_1 func = new Instrument_1();
        func.HelloWorld("Андрей");
        Console.WriteLine($"через 5 лет вам будет - {func.AgeToFive(18)}");
        Console.ReadLine();
    }
}
