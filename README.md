# Salario_final_vendedor
/*Uma revendedora de carros usados paga a seus funcionários vendedores um salário fixo por mês, mais uma comissão também fixa para cada carro vendido e mais 5% do valor das vendas por ele efetuadas.Escrever um algoritmo que leia o número de carros por ele vendidos, o valor total de suas vendas, o salário fixo e o valor que ele recebe por carro vendido. Calcule e escreva o salário final do vendedor.*/

using System;

namespace Salario_final_vendedor
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello!");

			Console.WriteLine("Digite o número de carros vendidos");
			string carvendstr = Console.ReadLine();
			decimal carvend = decimal.Parse(carvendstr);

			Console.WriteLine("Digite o o valor que o vendedor recebe por carro vendido");
			string comissaovendstr = Console.ReadLine();
			decimal comissaovend = decimal.Parse(comissaovendstr);

			Console.WriteLine("Digite o valor total de vendas");
			string valorvendstr = Console.ReadLine();
			decimal valorvend = decimal.Parse(valorvendstr);

			Console.WriteLine("Digite o salario fixo que o vendedor recebe");
			string venrecebstr = Console.ReadLine();
			decimal venreceb = decimal.Parse(venrecebstr);



			decimal salariofinal = venreceb + (comissaovend * carvend) + (valorvend / 100 * 5);

			Console.WriteLine("O salário final do vendedor será :" + salariofinal);

			Console.ReadKey();
		}
    }
}
