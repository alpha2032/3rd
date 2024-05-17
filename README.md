# 3rd
#compare two number and output the large one
class Comparision  
def initialize(no1,no2)  
@no1 = no1  
@no2 = no2  
end  
def compare_no  
@max = (@no1>@no2)? @no1:@no2  
puts("Greater number is  : #{@max}")  
end  
end  
puts("Enter 1st Number:")  
no1 = gets.chomp  
puts("Enter 2nd Number:")  
no2 = gets.chomp  
comparator = Comparision.new(no1,no2)  
comparator.compare_no 
