# Simple Calculator Android Application Using Android Studio

## Aim:
To create and design an Android application for a simple calculator using Android Studio with Java and XML.

## Equipments Required:
- Android Studio (Latest Version)
- Java
- XML
- Android Emulator or Android Device

## Algorithm:

**Step 1:** Open Android Studio and click on **File → New → New Project**.

**Step 2:** Enter the application name as `AndroidCalculator` and click Next.

**Step 3:** Select the Minimum SDK version and click Next.

**Step 4:** Select **Empty Views Activity** and click Finish.

**Step 5:** Design the calculator layout in the `activity_main.xml` file.

**Step 6:** Implement the calculator functionality in the `MainActivity.java` file.

**Step 7:** Add basic arithmetic operations such as:
- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)

**Step 8:** Save and run the application using an Android Emulator or physical Android device.

## Program:
Program to create and design a simple calculator Android application using **Java and XML** in Android Studio.

## Technologies Used:
- Java
- XML
- Android Studio

## Features:
- Simple user interface.
- Addition, subtraction, multiplication and division.
- Easy-to-use calculator buttons.

## Developed By:
**Name:** Iyyappan S <br>
**Register Number:** 212225230108 <br>
**Department:** Artificial Intelligence and Data Science <br>

Activity_Main.XML

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/display"
        android:layout_width="411dp"
        android:layout_height="wrap_content"
        android:gravity="center"
        android:padding="20dp"
        android:text="@string/Calculator"
        android:textSize="30sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@+id/editTextText"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <androidx.gridlayout.widget.GridLayout
        android:id="@+id/gridLayout2"
        android:layout_width="409dp"
        android:layout_height="425dp"
        android:layout_marginStart="2dp"
        android:layout_marginBottom="24dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent">

        <Button
            android:id="@+id/multiplication"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="X"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="6"
            app:layout_columnSpan="2"
            app:layout_row="1"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/clear"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="C"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="4"
            app:layout_columnSpan="2"
            app:layout_row="4"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/three"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="3"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="4"
            app:layout_columnSpan="2"
            app:layout_row="3"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/six"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="6"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="4"
            app:layout_columnSpan="2"
            app:layout_row="2"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/division"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="/"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="6"
            app:layout_columnSpan="2"
            app:layout_row="0"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/zero"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="0"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="0"
            app:layout_columnSpan="2"
            app:layout_row="4"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/equal"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="="
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="6"
            app:layout_columnSpan="2"
            app:layout_row="4"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/dot"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="."
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="2"
            app:layout_columnSpan="2"
            app:layout_row="4"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/one"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="1"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="0"
            app:layout_columnSpan="2"
            app:layout_row="3"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/addition"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="+"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="6"
            app:layout_columnSpan="2"
            app:layout_row="3"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/two"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="2"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="2"
            app:layout_columnSpan="2"
            app:layout_row="3"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/AllClear"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:layout_marginStart="10dp"
            android:layout_marginLeft="10dp"
            android:layout_marginTop="10dp"
            android:layout_marginEnd="10dp"
            android:layout_marginRight="10dp"
            android:layout_marginBottom="10dp"
            android:text="AC"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="0"
            app:layout_columnSpan="2"
            app:layout_row="0"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/modulus"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="%"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="4"
            app:layout_columnSpan="2"
            app:layout_row="0"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/fact"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="!"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="2"
            app:layout_columnSpan="2"
            app:layout_row="0"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/seven"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="7"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="0"
            app:layout_columnSpan="2"
            app:layout_row="1"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/nine"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="9"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="4"
            app:layout_columnSpan="2"
            app:layout_row="1"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/eight"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="8"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="2"
            app:layout_columnSpan="2"
            app:layout_row="1"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/five"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="5"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="2"
            app:layout_columnSpan="2"
            app:layout_row="2"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/four"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="4"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="0"
            app:layout_columnSpan="2"
            app:layout_row="2"
            app:layout_rowWeight="0" />

        <Button
            android:id="@+id/subtraction"
            android:layout_width="88dp"
            android:layout_height="70dp"
            android:layout_margin="5dp"
            android:text="-"
            android:textSize="30sp"
            app:cornerRadius="100dp"
            app:layout_column="6"
            app:layout_columnSpan="2"
            app:layout_row="2"
            app:layout_rowWeight="0" />

    </androidx.gridlayout.widget.GridLayout>

    <EditText
        android:id="@+id/editTextText"
        android:layout_width="0dp"
        android:layout_height="52dp"
        android:layout_marginLeft="25dp"
        android:layout_marginEnd="25dp"
        android:layout_marginBottom="44dp"
        android:ems="10"
        android:hint="0"
        android:inputType="text"
        android:text="0"
        android:textAlignment="textEnd"
        android:textSize="30sp"
        app:layout_constraintBottom_toTopOf="@+id/gridLayout2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

Mainactivity.java
```
package com.example.exp5_calculator;

import android.os.Bundle;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;


public class MainActivity extends AppCompatActivity {
    EditText editText;
    double firstNumber=0;
    String operator="";
    boolean newNumber=true;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        editText = findViewById(R.id.editTextText);

        // Number buttons
        int[] numberIds = {
                R.id.zero, R.id.one, R.id.two,
                R.id.three, R.id.four, R.id.five,
                R.id.six, R.id.seven, R.id.eight,
                R.id.nine
        };

        String[] numbers = {
                "0", "1", "2", "3", "4",
                "5", "6", "7", "8", "9"
        };

        for (int i = 0; i < numberIds.length; i++) {
            final String value = numbers[i];

            Button button = findViewById(numberIds[i]);

            button.setOnClickListener(v -> {
                if (newNumber) {
                    editText.setText(value);
                    newNumber = false;
                } else {
                    if (editText.getText().toString().equals("0")) {
                        editText.setText(value);
                    } else {
                        editText.append(value);
                    }
                }
            });
        }

        // Operator buttons
        findViewById(R.id.addition).setOnClickListener(v -> setOperator("+"));

        findViewById(R.id.subtraction).setOnClickListener(v -> setOperator("-"));

        findViewById(R.id.multiplication).setOnClickListener(v -> setOperator("*"));

        findViewById(R.id.division).setOnClickListener(v -> setOperator("/"));

        findViewById(R.id.modulus).setOnClickListener(v -> setOperator("%"));

        // Decimal button
        findViewById(R.id.dot).setOnClickListener(v -> {

            String value = editText.getText().toString();

            if (newNumber) {
                editText.setText("0.");
                newNumber = false;
            } else if (!value.contains(".")) {
                editText.append(".");
            }
        });

        // Equal button
        findViewById(R.id.equal).setOnClickListener(v -> calculate());

        // Clear button
        findViewById(R.id.clear).setOnClickListener(v -> {

            String value = editText.getText().toString();

            if (value.length() > 1) {
                editText.setText(value.substring(0, value.length() - 1));
            } else {
                editText.setText("0");
            }
        });

        // All Clear button
        findViewById(R.id.AllClear).setOnClickListener(v -> {

            editText.setText("0");
            firstNumber = 0;
            operator = "";
            newNumber = true;
        });

        // Factorial button
        findViewById(R.id.fact).setOnClickListener(v -> {

            try {
                double num = Double.parseDouble(
                        editText.getText().toString()
                );

                if (num < 0 || num != Math.floor(num) || num > 170) {
                    Toast.makeText(this,
                            "Enter an integer between 0 and 170",
                            Toast.LENGTH_SHORT).show();
                    return;
                }

                double result = 1;

                for (int i = 1; i <= (int) num; i++) {
                    result *= i;
                }

                editText.setText(formatResult(result));
                newNumber = true;

            } catch (Exception e) {
                editText.setText("Error");
                newNumber = true;
            }
        });
    }

    // Set mathematical operator
    private void setOperator(String op) {

        try {
            firstNumber = Double.parseDouble(
                    editText.getText().toString()
            );

            operator = op;
            newNumber = true;

        } catch (Exception e) {
            editText.setText("Error");
        }
    }

    // Perform calculation
    private void calculate() {

        if (operator.isEmpty()) {
            return;
        }

        try {
            double secondNumber = Double.parseDouble(
                    editText.getText().toString()
            );

            double result = 0;

            switch (operator) {

                case "+":
                    result = firstNumber + secondNumber;
                    break;

                case "-":
                    result = firstNumber - secondNumber;
                    break;

                case "*":
                    result = firstNumber * secondNumber;
                    break;

                case "/":

                    if (secondNumber == 0) {
                        editText.setText("Cannot divide by zero");
                        operator = "";
                        newNumber = true;
                        return;
                    }

                    result = firstNumber / secondNumber;
                    break;

                case "%":

                    if (secondNumber == 0) {
                        editText.setText("Cannot divide by zero");
                        operator = "";
                        newNumber = true;
                        return;
                    }

                    result = firstNumber % secondNumber;
                    break;
            }

            editText.setText(formatResult(result));

            firstNumber = result;
            operator = "";
            newNumber = true;

        } catch (Exception e) {

            editText.setText("Error");
            operator = "";
            newNumber = true;
        }
    }

    // Remove unnecessary decimal zeros
    private String formatResult(double result) {

        if (Double.isNaN(result) || Double.isInfinite(result)) {
            return "Error";
        }

        if (result == (long) result) {
            return String.valueOf((long) result);
        }

        return String.valueOf(result);
    }

}
```

Output Images:
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/212d3414-9273-4c77-bc54-f5f80b4cdf9e" />
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/558982b1-b369-4e9a-a222-c81745d59a84" />
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/a70a03cd-cb82-4633-bfbe-3160decdb35e" />
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/a702a8b9-fdee-4c59-a442-bed6dd55c3f9" />

## Result:
Thus a Simple Android Application create a simple calculator using Android Studio is developed and executed successfully
