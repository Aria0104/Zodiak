using System.Runtime.InteropServices;

Console.WriteLine("Ваше имя");
string name = Convert.ToString(Console.ReadLine());
Console.WriteLine("Ваша фамилия");
string surname  = Convert.ToString(Console.ReadLine());
Console.WriteLine("Дата рождения");
int date = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Месяц рождения");
int month = Convert.ToInt32(Console.ReadLine());

string zodiack = "";

if (((date >= 21 && date <= 31) && month == 3) || ((date <= 19 && date >=30) && month == 4))
{zodiack = "Овен"; }

if (((date >= 20 && date <= 30) && month == 4) || ((date <= 20 && date <= 31) && month == 5))
{ zodiack = "Телец"; }

if (((date >= 21 && date <= 31) && month == 5) || ((date <= 21 && date <= 30) && month == 6))
{ zodiack = "Близнецы"; }

if (((date >= 22 && date <= 30) && month == 6) || ((date <= 22 && date <= 31) && month == 7))
{ zodiack = "Рак"; }

if (((date >= 23 && date <= 31) && month == 7) || ((date <= 22 && date <= 31) && month == 8))
{ zodiack = "Лев"; }

if (((date >= 23 && date <= 31) && month == 8) || ((date <= 22 && date <= 30) && month == 9))
{ zodiack = "Дева"; }

if (((date >= 23 && date <= 30) && month == 9) || ((date <= 23 && date <= 31) && month == 10))
{ zodiack = "Весы"; }

if (((date >= 24 && date <= 31) && month == 10) || ((date <= 22 && date <= 30) && month == 11))
{ zodiack = "Скорпион"; }

if (((date >= 23 && date <= 30) && month == 11) || ((date <= 21 && date <= 31) && month == 12))
{ zodiack = "Стрелец"; }

if (((date >= 22 && date <= 31) && month == 12) || ((date <= 20 && date <= 31) && month == 1))
{ zodiack = "Козерог"; }

if (((date >= 21 && date <= 31) && month == 1) || ((date <= 18  && date <= 29) && month == 2))
{ zodiack = "Водолей"; }

if (((date >= 19 && date <= 29) && month == 2) || ((date <= 20 && date <= 31) && month == 3))
{ zodiack = "Рыбы"; }

Console.WriteLine($"Ваше имя: {name}, Ваша фамилия {surname}, Ваш знак зодиака {zodiack}");
