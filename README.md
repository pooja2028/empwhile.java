# empwhile.java
public class empwhile {

	public static final int part_time = 1;
        public static final int full_time = 2;
	public static final int wage_per_hour = 20;
        public static final int number_of_working_days=20;


	public static void main(String[] args) {
		int working_hours = 0;
		int number_of_working_hours=100;
		int salary = 0;
		int totalsalary = 0;
		int workingdays=0; 
			while  ( working_hours <= number_of_working_hours && workingdays <  number_of_working_days ) {
				workingdays++;
			 int empcheck = (int) Math.floor(Math.random() * 10) % 3;

			switch (empcheck) {
			case part_time:
			working_hours=4;
			break;
			case full_time:
			working_hours=8;
			break;
			default:
			working_hours=0;
		}		
			salary = working_hours * wage_per_hour;
			totalsalary += salary;
			number_of_working_hours += working_hours;
			System.out.println(" Employee wage is: " +salary);
		}
			 System.out.println(" Employee totalsalary is: " +totalsalary);
	}

}
