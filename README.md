<p align="center">
<p align="center">
  <a href="https://github.com/i-rin-eam">
    <img src="https://avatars.githubusercontent.com/u/154800878?s=400&u=5d18880cc28646190a19a971bfcdbc54644eab07&v=4" alt="Logo" width="100" height="100">
  </a> 
<h1 align='center'>Practice Challenge 1 Soltuion</h1>
<h3 align='center'>
   Visit my youtube channel <a href="https://www.youtube.com/@LearnWithYeamin">Learn With Yeamin</a>
</h3>
</p>

## Step 1: Here is `activity_main.xml` code.
```xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#ECEFF1"
    android:padding="16dp">

    <!-- Display for Calculator -->
    <EditText
        android:id="@+id/editTextResult"
        android:layout_width="match_parent"
        android:layout_height="150dp"
        android:layout_alignParentTop="true"
        android:layout_marginBottom="10dp"
        android:background="#FFFFFF"
        android:elevation="4dp"
        android:gravity="end|bottom"
        android:hint="0"
        android:inputType="none"
        android:padding="10dp"
        android:textColor="#000"
        android:textSize="24sp"
        android:textStyle="bold" />

    <!-- Buttons Layout -->
    <LinearLayout
        android:id="@+id/buttonLayout"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_below="@+id/editTextResult"
        android:layout_alignParentBottom="true"
        android:layout_marginTop="10dp"
        android:orientation="vertical">

        <!-- Row 1 -->
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:gravity="center"
            android:orientation="horizontal">

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnClear"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FF7043"
                android:text="C"
                android:textColor="#FFF"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnDivide"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FFAB40"
                android:text="÷"
                android:textColor="#FFF"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnMultiply"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FFAB40"
                android:text="×"
                android:textColor="#FFF"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnDelete"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FF7043"
                android:text="⌫"
                android:textColor="#FFF"
                android:textSize="24sp" />
        </LinearLayout>

        <!-- Row 2 -->
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:gravity="center"
            android:orientation="horizontal">

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn7"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="7"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn8"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="8"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn9"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="9"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnSubtract"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FFAB40"
                android:text="-"
                android:textColor="#FFF"
                android:textSize="24sp" />
        </LinearLayout>

        <!-- Row 3 -->
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:gravity="center"
            android:orientation="horizontal">

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn4"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="4"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn5"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="5"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn6"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="6"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnAdd"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FFAB40"
                android:text="+"
                android:textColor="#FFF"
                android:textSize="24sp" />
        </LinearLayout>

        <!-- Row 4 -->
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:gravity="center"
            android:orientation="horizontal">

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn1"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="1"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn2"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="2"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn3"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="3"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnEquals"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#FF7043"
                android:text="="
                android:textColor="#FFF"
                android:textSize="24sp" />
        </LinearLayout>

        <!-- Row 5 -->
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:gravity="center"
            android:orientation="horizontal">

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btn0"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="2"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="0"
                android:textColor="#000"
                android:textSize="24sp" />

            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/btnDecimal"
                android:layout_width="0dp"
                android:layout_height="match_parent"
                android:layout_weight="1"
                android:layout_margin="4dp"
                android:background="#ECEFF1"
                android:text="."
                android:textColor="#000"
                android:textSize="24sp" />
        </LinearLayout>

    </LinearLayout>

</RelativeLayout>
```
## Authors

**MD YEAMIN** - Android Software Developer <a href="https://www.youtube.com/@LearnWithYeamin">**(Learn With Yeamin)**</a> 

<h1 align="center">Thank You ❤️</h1>
