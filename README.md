# usageCode
some code

example:
string count(string f){//num add
     int q = f.length();
     int k = f[q-1]-'0';
     if(9 != k){
         k+=1;
         f[q-1] = k;
     }else{
         f[f.length()-1] = '0';
         for(int i=0;i<q;i++){
             if('9' == f[q-1-i]){
                 f[q-1-i] = '0';
             }else{
                 f[q-1-i] = f[q-1-i]-'0'+1;
             }
         }
     }
     if(0 == f[0]){
         f[0] = '1';
     }
     return f;
}

