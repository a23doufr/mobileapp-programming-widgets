
# Rapport
The code below was added by dragging from the design-window in activity_main.xml. 
It is the Constraint Layout and is constraint to all sides of the parent layout with some
horizontal and vertical bias.
```
<androidx.constraintlayout.widget.ConstraintLayout

//Rest of code for its position and the contained widgets ...

</androidx.constraintlayout.widget.ConstraintLayout>
```

Inside the ConstraintLayout a TextView was added and constrained to the sides and top of the 
parent Layout. Below is the code for the constraints of the TextView.
```
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toTopOf="parent" />
```

Then I moved the TextView down by adding some top margin, and adding a Button with it's 
sides constrained to the TextViews sides which aligns them vertically. The top of the button
is also constrained to the bottom of the textView with a 10 dp margin.
```
app:layout_constraintEnd_toEndOf="@+id/textView5"
app:layout_constraintStart_toStartOf="@+id/textView5"
app:layout_constraintTop_toBottomOf="@+id/textView5" />
```

Then a Switch is added with the same constrains towards the Button as the Button has 
towards he TextView.
```
app:layout_constraintEnd_toEndOf="@+id/button6"
app:layout_constraintStart_toStartOf="@+id/button6"
app:layout_constraintTop_toBottomOf="@+id/button6" />
```
Lastly some text inside the widgets were changed.








![](Screenshotconstraint.png)


