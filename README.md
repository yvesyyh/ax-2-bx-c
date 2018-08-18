# ax-2-bx-c
import math
def quadratic(a,b,c):
	
	if a == 0 :
		return ((-1)*c)/b
	d=b**2-4*a*c
	if d>0:
		sqrt_d=math.sqrt(d)
		if sqrt_d>0:
			x1=(-b+sqrt_d)/2*a
			x2=(-b-sqrt_d)/2*a
			return x1,x2
		elif d=0:
			x =-b/2*a
			return x
		else:
			return 'no results'      

if __name__ == '__main__':
	a=int(input('please enter a number not 0: '))
	b=int(input('please enter a number: '))
	c=int(input('please enter a number: '))
	print(quadratic(a,b,c))
