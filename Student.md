public class Student {
   //Instance variables
    private String name;
    private double average;

    //Constructor
    public Student(String name, double average){//creates student object
        //will run when you create a new student object
        //constructor, has the same name as the class
        //double is a data type, one of the eight, twice the size of a float
        this.name = name; //set instance variable


        //validate that average is >(positive) 0.0 and <= 100.0; otherwise
        //keep instance variable average's default value (0,0)
        if (average > 0.0){
            if(average <= 100.00){
                this.average = average; //take the value and assign it to the average
            }
        }
    }//END Constructor : Student
    /////////////////////////////////////////////////////////////////
    public void setName(String name) {
        this.name = name;
    }
    ////////////////////////////////////////////////////////////////
    public String getName() {
        return name;
        //no void because its actually returning a value
    }
//Set the student's Average.
    public void setAverage(double average) {

        //validate that average is >(positive) 0.0 and <= 100.0; otherwise
        //keep instance variable average's default value (0,0)
        if (average > 0.0){
            if(average <= 100.00){
                this.average = average; //take the value and assign it to the average
            }
        }
    }//set average
///////////////////
    public double getAverage() {
        return average;
    }

    //this converts the average to a letter grade.
public String getLetterGrade(){ //letterGrade is a string, not an object
        String letterGrade = ""; //null, so it can be set by the if statements

        //Map the letter grade to the average
    if (average >= 90) {
        letterGrade = "A";
    }
    else if(average>= 80.0){
        letterGrade = "B";
    }
    else if(average >= 70) {
        letterGrade = "C";
    }
    else if(average>= 60.0){
        letterGrade = "D";
    }
    else {
        letterGrade = "F";
    }
    return letterGrade;
    }
}//End Class: Student
