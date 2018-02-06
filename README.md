# MyPr-001   

#! /usr/bin/python3            

# 导入工具，减少代码阅读 
import cards_tools

# 无限循环，由用户主动决定什么时候退出系统
while True:

    # TODO 显示功能菜单
    cards_tools.show_menu()
    
    action_str = input("请选择希望执行的操作：")
    print("您选择的操作是【%s】" % action_str)

    # 1.2.3 针对名片的操作
    if action_str in ["1","2","3"]:  # in 成员字符
        # pass 具体操作预留代码
        
        # 新增名片
        if action_str == "1":
            # pass 具体操作预留代码
            cards_tools.new_card()
            
        # 显示全部
        elif action_str == "2":
            # pass 具体操作预留代码
            cards_tools.show_all()
            
        # 查询名片
        elif action_str == "3":
            #pass 具体操作预留代码
            cards_tools.search_card()
            
    # 0 退出系统
    elif action_str == "0":
        print("欢迎再次使用【名片管理系统】")
        break
        
    # 其他内容输入错误，需要提示用户
    else:
        print("您输入的不正确，请重新选择")
