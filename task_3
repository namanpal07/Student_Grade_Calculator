# Student_Grade_Calculator
import java.util.Scanner;

public class GradeCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input: number of subjects
        System.out.print("Enter the number of subjects: ");
        int numSubjects = sc.nextInt();

        int[] marks = new int[numSubjects];
        int total = 0;

        // Input: marks for each subject
        for (int i = 0; i < numSubjects; i++) {
            System.out.print("Enter marks for Subject " + (i + 1) + " (out of 100): ");
            marks[i] = sc.nextInt();
            
            // Optional: Validate marks
            if (marks[i] < 0 || marks[i] > 100) {
                System.out.println("Invalid marks entered. Please enter between 0 and 100.");
                i--; // re-enter
                continue;
            }
            total += marks[i];
        }

        // Calculate average
        double average = (double) total / numSubjects;

        // Determine grade
        String grade;
        if (average >= 90) {
            grade = "A+";
        } else if (average >= 80) {
            grade = "A";
        } else if (average >= 70) {
            grade = "B";
        } else if (average >= 60) {
            grade = "C";
        } else if (average >= 50) {
            grade = "D";
        } else {
            grade = "F (Fail)";
        }

        // Display results
        System.out.println("\n--- Student Grade Report ---");
        System.out.println("Total Marks: " + total + " out of " + (numSubjects * 100));
        System.out.printf("Average Percentage: %.2f%%\n", average);
        System.out.println("Grade: " + grade);

        sc.close();
    }
}
