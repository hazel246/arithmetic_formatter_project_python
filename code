def arithmetic_arranger(problems, show_answers=False):

    if len(problems) >5:
        return 'Error: Too many problems.'

    top=[]
    below=[]
    dashes=[]
    output=[]

        #splitting the problem into 3 components
    for p in problems:
            parts=p.split()
            if len(parts)!=3:
                return "Each problem should have 2 operands and 1 operator"

            n1,operator,n2=parts

            if operator not in ('+', '-'):
                return "Error: Operator must be '+' or '-'."

            if n1.isdigit()==False or n2.isdigit()==False :
                return "Error: Numbers must only contain digits."

            if len(n1)>4 or len(n2)>4:
                return "Error: Numbers cannot be more than four digits."

            
            if operator=='+':
                ans=str(int(n1)+int(n2))
            elif operator =='-':
                ans=str(int(n1)-int(n2))

            
            width=max(len(n1),len(n2))+2 #+2 for operator and space

            top.append(n1.rjust(width))
            below.append(operator +' '+n2.rjust(width-2))
            dashes.append('-'*width)
            output.append(ans.rjust(width))

    arranged_problems='    '.join(top) + '\n' + '    '.join(below) + '\n' +'    '.join(dashes)

    if show_answers:
                arranged_problems += '\n' + '    '.join(output)


    return arranged_problems


            






    

print(arithmetic_arranger(["32 + 698", "3801 - 2", "45 + 43", "123 + 49"]))
print(arithmetic_arranger(["3 + 855", "988 + 40"], True))



print(arithmetic_arranger(["3 / 855", "3801 - 2", "45 + 43", "123 + 49"]))

print(arithmetic_arranger(["24 + 85215", "3801 - 2", "45 + 43", "123 + 49"]))

print(arithmetic_arranger(["98 + 3g5", "3801 - 2", "45 + 43", "123 + 49"]))
