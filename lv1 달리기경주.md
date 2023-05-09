<img width="80%" src="https://user-images.githubusercontent.com/109085338/236971787-d5dc7c38-51c3-4743-b04c-f45d987464e3.png"/>

---------------------------------------------------------------------------------------------------------------------------

import java.util.*;

class Solution {
    public String[] solution(String[] players, String[] callings) {
      //  String[] answer = {};
        
        
        
        for(int i = 0; i < callings.length; i++){
            int num = Arrays.asList(players).indexOf(callings[i]); 
            String a = players[num];
            String b = players[num-1];
            players[num] = b;
            players[num-1] = a;
        }
        
        
        String[] answer = players.clone();
        return answer;
        
    }
}
