# package AssignmentPack;

import java.util.Scanner;

public class Ses2Assignment4 {
	static int days = 0;

	public static int month2Days(String str) {

		switch (str) {
		case "January":
			days = 31;
			break;
		case "February":
			days = 28;
			break;
		case "March":
			days = 31;
			break;
		case "April":
			days = 30;
			break;
		case "May":
			days = 31;
			break;
		case "June":
			days = 30;
			break;
		case "July":
			days = 31;
			break;
		case "August":
			days = 31;
			break;
		case "September":
			days = 30;
			break;
		case "October":
			days = 31;
			break;
		case "November":
			days = 30;
			break;
		case "December":
			days = 31;
			break;
		default:
			System.out.println("Invalid Month entry...");
			break;
		}
		return days;

	}

	public static void main(String[] args) {
		System.out.print("Enter the month: ");
		Scanner sc = new Scanner(System.in);
		String inp = sc.nextLine();

		Ses2Assignment4.month2Days(inp);
		if (days == 0) {
			System.out.println("");
		} else
			System.out.println("No of days in " + inp + " month is " + days);

	}
}
