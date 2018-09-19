# P05-DiazUriasJorgeDavid
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Diagnostics;

namespace TiempoEjecucion
{
    class Program
    {
        static void Main(string[] args)
        {
            double suma = 0;
            Stopwatch stopwatch = Stopwatch.StartNew();
            for (double i = 0; i <= 1000000; i++)
            {
                suma = suma + i;
            }
            Console.WriteLine("La suma de los numeros del 1 al 1000000 es {0} \nTiempo 
            Transcurrido: {1}", suma, stopwatch.Elapsed);
            Console.ReadKey();
        }
    }
}
