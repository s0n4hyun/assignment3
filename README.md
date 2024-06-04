# assignment3

def divide_numbers():

    try:
    
        # 사용자로부터 두 개의 자연수를 입력받습니다.
        
        dividend = int(input("나눠지는 수를 입력하세요: "))
        
        divisor = int(input("나누는 수를 입력하세요: "))
        


        # 입력받은 두 수로 나눗셈을 실행합니다.
        
        result = dividend / divisor
        
        
        print(f"{dividend}을(를) {divisor}로 나눈 결과는 {result}입니다.")

    
    
    except ValueError:
    
        # 입력이 자연수가 아닌 경우에 대한 예외 처리
        
        print("잘못된 입력입니다. 자연수를 입력하세요.")

    
    
    except ZeroDivisionError:
    
        # 나누는 수가 0인 경우에 대한 예외 처리
        
        print("0으로 나눌 수 없습니다. 다른 수를 입력하세요.")



    except Exception as e:
    
        # 기타 예외 발생 시 처리
        
        print("오류가 발생했습니다:", e)



# 함수 호출

divide_numbers()
