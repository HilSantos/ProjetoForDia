# ProjetoForDia
Idem.

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ProjetoForDia
{
    public class Program
    {
        static void Main(string[] args)
        {
            /*Solicite e receba o nome, a cidade, e a idade da pessoa e exiba
             * as informações. Faça esta repetição para quatro pessoas.
            */
            string nome, cidade;
            int idade;

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine("Informe seu nome: ");
                nome = Console.ReadLine();

                Console.WriteLine("Informe a cidade: ");
                cidade = Console.ReadLine();

                Console.WriteLine("Digite o ano de nascimento do usuario: ");
                idade = Convert.ToInt32(Console.ReadLine());

                idade = DateTime.Now.Year - idade;
                Console.WriteLine("Nome: " + nome);
                Console.WriteLine("Idade: " + idade);
            }

                Console.ReadKey();
        }
    }
}
