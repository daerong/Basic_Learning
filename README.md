## C++
**Include**

    #include <iostream>
    // cout, cin, cerr ...
    #include <algorithm>
    // min(), max(), abs() ...
    #include <string>
    // string, strlen(), strcpy(), strcmp() ...

**Increasing speed**

    #define endl "\n"			// endl보다 '/n'이 빠름
    
    int main(){
	    ios_base::sync_with_stdio(false);		// stdio와의 sync를 끊는다.
	    cin.tie(NULL);							// cin을 cout으로부터 untie합니다.
	    cout.tie(NULL);							// cout을 cin으로부터 untie합니다.
	    
	    return 0;
    }
