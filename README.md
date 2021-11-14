# 2021-02-database

## week3 실습 실행 방법
1. 레포지토리 복사(wsl 환경에서 명령어 입력)
   - (SSH 설정한 경우) git clone git@github.com:riven1211/2021_DB_test.git
   - (token을 사용하는 경우) git clone https://github.com/riven1211/2021_DB_test.git
2. week3 폴더로 이동
    > cd week3
3. 콘솔창(powershell)에서 npm package 설치
    > npm install
4. database/sql.js에서 본인의 데이터베이스 정보 입력(주석부분)
<pre>
<code>
const pool = mysql.createPool(
    process,env.JAWSDB_URL ?? {
        host : 'localhost',
        user : 'root', // 본인의 mysql user id
        database : 'tutorial', // 본인이 만들 데이터베이스 이름
        password : 'password',  // 본인의 mysql password
        waitForConnections : true,
        connectionLimit: 10,
        queueLimit : 0
    }
);
</code>
</pre>

<br>
## <span style="color:red">테이블 작성법</span>

이름|과|전공|학번
---|---|---|---|
강현승|정보통신공학과|정보통신|12161680|
##

# week11_3
