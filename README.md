using System;

class WeatherMoodApp
{
    static void Main(string[] args)
    {
        Console.WriteLine("=== Weather Mood Suggestion App ===");

        while (true)
        {
            Console.Write("\nEnter the weather (sunny, rainy, snowy, cloudy, exit): ");
            string weather = Console.ReadLine().ToLower();

            if (weather == "exit")
            {
                Console.WriteLine("Goodbye!");
                break;
            }

            switch (weather)
            {
                case "sunny":
                    Console.WriteLine("☀️ It's a great day for a walk, biking, or reading outside!");
                    break;
                case "rainy":
                    Console.WriteLine("🌧 Perfect day for movies, coding, or a warm drink indoors.");
                    break;
                case "snowy":
                    Console.WriteLine("❄️ Go skiing, build a snowman, or cozy up with hot chocolate!");
                    break;
                case "cloudy":
                    Console.WriteLine("☁️ Great time for reflection, writing, or light exercise.");
                    break;
                default:
                    Console.WriteLine("🤔 I don’t know that weather type. Try sunny, rainy, snowy, or cloudy.");
                    break;
            }
        }
    }
}
