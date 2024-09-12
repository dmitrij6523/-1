

internal class Program
{
    private static void Main(string[] args)
    {
    first:
        double a;
        double b;
        char oper;
        Console.WriteLine("Введите первое число: ");
        a = Convert.ToDouble(Console.ReadLine());

        Console.WriteLine("Введите оператор: ");
        oper = Convert.ToChar(Console.ReadLine());

        Console.WriteLine("Введите второе число: ");
        b = Convert.ToDouble(Console.ReadLine());

        if (oper == '+')
        {
            Console.WriteLine(a + b);
            goto first;
        }
        else if (oper == '-')
        {
            Console.WriteLine(a - b);
            goto first;
        }
        else if (oper == '*')
        {
          
            Console.WriteLine(a * b);
            goto first;
        }
        else if (oper == '/')
        {
           
            Console.WriteLine(a / b );
            goto first;
        }
        else
        {
            Console.WriteLine("Неизвестный оператор");
            goto first;
        }
    }
}
