//Adrian Paul D. Peralta
//BSCpE 1-1
//ArtistWiki
using System;
using System.Collections.Generic;

namespace ArtistWiki
{
	class Program
	{
		static void Main(string[] args)
		{
			int selection = 0;
			while (selection != 6)
			{
				Console.WriteLine("Pick a group:");
				Console.WriteLine("1. LE SSERAFIM");
				Console.Write("Enter your selection: ");

				string userInput = Console.ReadLine();

				while (userInput != "0")
				{
					if (userInput == "1")
					{
						List<string> tracks = new List<string>
						{
							"Fearless (2022)",
							"Antifragile (2022)",
							"Unforgiven (2023)"
						};

						Console.WriteLine("\nLE SSERAFIM Title Tracks:");
						foreach (var track in tracks)
						{
							Console.WriteLine("- " + track);
						}

						Console.WriteLine("\nLE SSERAFIM WIKI");
						Console.WriteLine("Select a member:");
						Console.WriteLine("1. Chaewon");
						Console.WriteLine("2. Sakura");
						Console.WriteLine("3. Yunjin");
						Console.WriteLine("4. Kazuha");
						Console.WriteLine("5. Eunchae");
						Console.WriteLine("6. Exit the program.");
						Console.Write("Enter your selection: ");

						userInput = Console.ReadLine();
						switch (userInput)
						{
							case "1":
								Console.WriteLine("Stage Name: Chaewon");
								Console.WriteLine("Birth Name: Kim Chaewon (김채원)");
								Console.WriteLine("Position: Leader, Vocalist");
								Console.WriteLine("Birthday: August 1, 2000");
								Console.WriteLine("Nationality: Korean");
								Console.WriteLine("Instagram: @_chaechae_1");
								Console.WriteLine("MBTI: ISTP");
								Console.WriteLine("Former IZ*ONE member");
								break;

							case "2":
								Console.WriteLine("Stage Name: Sakura");
								Console.WriteLine("Birth Name: Miyawaki Sakura (宮脇 咲良)");
								Console.WriteLine("Position: Vocalist");
								Console.WriteLine("Birthday: March 19, 1998");
								Console.WriteLine("Nationality: Japanese");
								Console.WriteLine("Instagram: @39saku_chan");
								Console.WriteLine("MBTI: INTP");
								Console.WriteLine("Former IZ*ONE member");
								break;

							case "3":
								Console.WriteLine("Stage Name: Yunjin");
								Console.WriteLine("Birth Name: Huh Yunjin (허윤진)");
								Console.WriteLine("Position: Vocalist");
								Console.WriteLine("Birthday: October 8, 2001");
								Console.WriteLine("Nationality: Korean-American");
								Console.WriteLine("Instagram: @jenaissante");
								Console.WriteLine("MBTI: ENFJ");
								break;

							case "4":
								Console.WriteLine("Stage Name: Kazuha");
								Console.WriteLine("Birth Name: Nakamura Kazuha (中村 一葉)");
								Console.WriteLine("Position: Sub-Vocalist, Rapper, Dancer");
								Console.WriteLine("Birthday: August 9, 2003");
								Console.WriteLine("Nationality: Japanese");
								Console.WriteLine("Instagram: @k_a_z_u_h_a__");
								Console.WriteLine("MBTI: INFP");
								break;

							case "5":
								Console.WriteLine("Stage Name: Eunchae");
								Console.WriteLine("Birth Name: Hong Eunchae (홍은채)");
								Console.WriteLine("Position: Vocalist, Lead Dancer, Maknae");
								Console.WriteLine("Birthday: November 10, 2006");
								Console.WriteLine("Nationality: Korean");
								Console.WriteLine("Instagram: @hhh.e_c.v");
								Console.WriteLine("MBTI: ISFJ");
								break;

							case "6":
								Console.WriteLine("Goodbye!");
								return;

							default:
								Console.WriteLine("Invalid input, Please try again.");
								break;
						}
					}
				}
			}
		}
	}
}
