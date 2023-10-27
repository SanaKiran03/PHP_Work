<?php

function calGrade($percentage)
{
    if ($percentage >= 90) {
        echo 'A';
    } elseif ($percentage >= 80) {
        echo'B';
    } elseif ($percentage >= 70) {
        echo 'C';
    } elseif ($percentage >= 60) {
        echo 'D';
    } else {
        echo 'F';
    }
}

function Marksheet($studentName, $subject1, $subject2, $subject3, $subject4, $subject5)
{
    $totalMarks = $subject1 + $subject2 + $subject3 + $subject4 + $subject5;
    $totalSubjects = 5;
    $percentage = ($totalMarks / ($totalSubjects * 100)) * 100;
    $grade = calGrade($percentage);

    echo "Student Name: $studentName <br>";
    echo "------------------------<br>";
    echo "Subject Marks <br>";
    echo "------------------------<br>";
    echo "Subject 1: $subject1<br>";
    echo "Subject 2: $subject2<br>";
    echo "Subject 3: $subject3<br>";
    echo "Subject 4: $subject4<br>";
    echo "Subject 5: $subject5<br>";
    echo "------------------------<br>";
    echo "Total Marks: $totalMarks<br>";
    echo "Percentage: $percentage%<br>";
    echo "Grade: $grade <br>";
}


?>
