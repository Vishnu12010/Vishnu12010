package com.vishnu.jsp;

import java.util.Scanner;

public class StudentGrades {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String[] studentNames = new String[10];
        double[] attendancePercentages = new double[10];

        
        for (int i = 0; i < 10; i++) {
            System.out.print("Enter the name of student " + (i + 1) + ": ");
            studentNames[i] = scanner.nextLine();
            System.out.print("Enter the attendance percentage for " + studentNames[i] + ": ");
            attendancePercentages[i] = scanner.nextDouble();
            scanner.nextLine();
        }

        
        System.out.println("\nGrades for the students:");

        for (int i = 0; i < 10; i++) {
            System.out.print(studentNames[i] + ": ");
            switch ((int) attendancePercentages[i]) {
                case 90:
                case 91:
                case 92:
                case 93:
                case 94:
                case 95:
                case 96:
                case 97:
                case 98:
                case 99:
                case 100:
                    System.out.println("A");
                    break;
                case 80:
                case 81:
                case 82:
                case 83:
                case 84:
                case 85:
                case 86:
                case 87:
                case 88:
                case 89:
                    System.out.println("B");
                    break;
                case 70:
                case 71:
                case 72:
                case 73:
                case 74:
                case 75:
                case 76:
                case 77:
                case 78:
                case 79:
                    System.out.println("C");
                    break;
                case 60:
                case 61:
                case 62:
                case 63:
                case 64:
                case 65:
                case 66:
                case 67:
                case 68:
                case 69:
                    System.out.println("D");
                    break;
                case 45:
                case 46:
                case 47:
                case 48:
                case 49:
                case 50:
                case 51:
                case 52:
                case 53:
                case 54:
                case 55:
                case 56:
                case 57:
                case 58:
                case 59:
                    System.out.println("E");
                    break;
                default:
                    System.out.println("F");
                    break;
            }
        }

        scanner.close();
    }
}
