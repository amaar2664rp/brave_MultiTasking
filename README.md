# brave_MultiTasking
#include &lt;MultiTasking.au3> _Task_Create("Task1","Working_Function") _Task_Join("Task1") _Task_Create("Task2","Not_Working_function")  func ToBeCalled() Msgbox(0,"Task"," Working !") endfunc  func Working_Function() TobeCalled() endfunc  func Not_Working_function() _Task_Create("","ToBeCalled") endfunc
