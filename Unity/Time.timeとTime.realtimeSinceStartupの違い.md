Time.timeは同一フレーム内で取得した値は同じになる。
Time.realtimeSinceStartupは同一フレーム内でもリアルタイムの時間情報になる。

(例)
void Hoge()
{
  Debug.Log( "Time.realtimeSinceStartup:1 = " + Time.realtimeSinceStartup +
            " , Time.realtimeSinceStartup:2 = " + Time.realtimeSinceStartup +
            " , Time.time:1 = " + Time.time +
            " , Time.time:2 = " + Time.time);
}

<結果>
３フレーム分
Time.realtimeSinceStartup:1 = 3.114911 , Time.realtimeSinceStartup:2 = 3.114912 , Time.time:1 = 3.083903 , Time.time:2 = 3.083903
Time.realtimeSinceStartup:1 = 3.131449 , Time.realtimeSinceStartup:2 = 3.13145 , Time.time:1 = 3.100469 , Time.time:2 = 3.100469
Time.realtimeSinceStartup:1 = 3.147841 , Time.realtimeSinceStartup:2 = 3.147842 , Time.time:1 = 3.117036 , Time.time:2 = 3.117036

参考サイト:http://ftvoid.com/blog/post/677