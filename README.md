一个linux Server程序的epoll实现

    程序有2个瓶颈：
    
    1.内部的锁会造成多线程共享epoll描述符的锁竞争
    
    2.短连接建立能力差,未经过优化网络参数,只能达到3万/秒的建立能力
    
