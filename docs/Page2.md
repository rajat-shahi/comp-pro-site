# Templates and completions

==Github repository link :==
<br>
`https://github.com/rajat-shahi/comp-pro-library/tree/main/template%20and%20completions`

### initial template for comp-pro

```cpp title="basic-template.cpp" linenums="1"
#include <bits/stdc++.h>
using namespace std;

#ifndef ONLINE_JUDGE
#include"/Users/rajat.shahi/Desktop/CPP/debug.h"
#endif
#ifdef ONLINE_JUDGE
#define debug(...) 42
#endif

#define endl '\n'
const int mod = 1e9 + 7;
// const int mod = (119 << 23) + 1;
#define rep(i,a,b) for(auto i=a;i<=b;i++)
#define per(i,a,b) for(auto i=a;i>=b;i--)
using ll = long long;
using vll = vector<long long>;
using vi = vector<int>;
using pii = pair<int, int>;
using pll = pair<ll, ll>;
#define all(x) x.begin(), x.end()
#define rall(x) x.rbegin(), x.rend()
#define sz(x) (int) x.size()
#define pb push_back
#define ff first
#define ss second
const int MAXN = 2e5 + 5;
const int inf = 1001001001;
const long long INF = 1001001001001001001ll;



int main() {

	cin.tie(0)->sync_with_stdio(0);
	cin.exceptions(ios::badbit | ios::failbit);

	

	return 0;
}
```

<br><br>

### debugging template for competitive programming

```cpp title="debug.h" linenums="1"
string to_string(string s)
{
    return '"' + s + '"';
}
string to_string(const char *s)
{
    return to_string((string) s);
}
string to_string(bool b)
{
    return (b ? "true" : "false");
}
template <typename A, typename B>
string to_string(pair<A, B> p)
{
    return "(" + to_string(p.first) + ", " + to_string(p.second) + ")";
}
template <typename A>
string to_string(A v)
{
    bool first = true;
    string res = "{";
    for (const auto &x : v)
    {
        if (!first)
        {
            res += ", ";
        }
        first = false;
        res += to_string(x);
    }
    res += "}";
    return res;
}
void debug_out()
{
    cerr << endl;
}
template <typename Head, typename... Tail>
void debug_out(Head H, Tail... T)
{
    cerr << " " << to_string(H);
    debug_out(T...);
}

template<typename T>
void debug_out(queue<T> q)
{
    cerr << "{ ";
    while(not q.empty())
    {
        cerr << q.front() << " , ";
        q.pop();
    }
    cerr << "}";
}

template<typename T>
void debug_out(stack<T> st)
{
    cerr << "{ ";
    while(not st.empty())
    {
        cerr << st.top() << " , ";
        st.pop();
    }
    cerr << "}";
}

template<typename T>
void debug_out(priority_queue<T> pq)
{
    cerr << "{ ";
    while(not pq.empty())
    {
        cerr << pq.front() << " , ";
        pq.pop();
    }
    cerr << "}";
}

void debug_out(string str)
{
    cerr << str << endl;
}


#ifndef ONLINE_JUDGE
#define debug(...) cerr << "Line " << __LINE__ << ": "<< "[" << #__VA_ARGS__ << "]:", debug_out(__VA_ARGS__)
#else
#define debug(...) 42
#endif
```
<br><br>
