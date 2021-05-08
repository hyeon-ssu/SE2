# SE2 - https://github.com/hyeon-ssu/SE2

---
## **목차**  
- [first-commit](#first-commit)  
-  second commit  
- third commit  
- fourth commit  
- fifth commit  
- git 명령어 사용 표  

---

### **1. first commit**  
**init :** 이번 과제는 git을 사용하는 과제이기 때문에 터미널을 열어 `git init` 명령어를 사용해 로컬 저장소를 생성합니다.  
  
  
**config :** `git config --global user.name "이름"` 명령어를 사용해 이름을 설정하고, `git config --global user.email "이메일"` 명령어를 사용해 이메일을 설정합니다. 한 번 이 명령어를 사용하면 다시 사용할 일이 거의 없습니다. 그리고 **git config user.name** 이나 **git config user.email**을 사용해 이름과 이메일을 확인할 수 있습니다.  
  
  
![init+config](https://postfiles.pstatic.net/MjAyMTA1MDhfNzAg/MDAxNjIwNDY5NzYxNzQ2.DKXoZqX-YwLsUFm1IxFoPMBfcexeHqj9kW1a71L2f54g.9SCSkAJYtwv82F97jwiJxVs1uhI2XGaRfTk2jjDILe4g.PNG.angelcup2001/init+config.png?type=w773)  
  
  
![config](https://postfiles.pstatic.net/MjAyMTA1MDhfNDUg/MDAxNjIwNDY5Nzg1NzQ0.XTWUS_GqHzi9L2o9Ab46EEgbmRVoG0xY0w3ef7Jsmjog.GvXqSIWRtO8h8Qo-SG7e96hBtYVv_eZFlU2AVeSNOL0g.PNG.angelcup2001/config.png?type=w773)  
  
  
**clone :** `git clone 주소` 명령어를 통해 프로젝트를 복제할 수 있습니다. 이번 과제에서는 저의 github를 복제했습니다.  
  
  
![clone](https://postfiles.pstatic.net/MjAyMTA1MDhfMjky/MDAxNjIwNDY5ODA0MTIx.cgquDnRLaR9AxIk2rOVZ6_Lad0v8uSWKjQCmSIYKHbwg.FATZq-u5B9prqiGURttJIAfcEEmRI1FTD4ZPYZr4uVMg.PNG.angelcup2001/clone.png?type=w773)  
  
  
**add :** 과제를 작성하다보니 과제 파일을 저장하고 싶습니다. 저장하기 위해서 우선 `git add 파일` 명령어를 통해 파일을 스테이징 할 수 있습니다. Git의 Repository 구조는 크게 작업폴더(Working directory) > 인덱스(Staging Area) > 저장소(Head -Repository)로 구성되어 있습니다. 파일을 커밋하기 위해선 Staging Area인 인덱스에 보내야 하는데 그 것을 '스테이징 한다'고 합니다. 또한 **git add -A** 명령어를 사용하면 스테이징 하지 않은 파일 전부를 스테이징 시킵니다.  
  
  
**status :** 그 다음 `git status` 명령어를 통해 현재 상태를 확인할 수 있습니다. 현재 내 파일이 스테이징이 되었는지 되지 않았는지 확인할 수 있습니다.  
  
  
![add+status](https://postfiles.pstatic.net/MjAyMTA1MDhfMTE4/MDAxNjIwNDY5ODE3Nzc5.mKzaiUCUXf2-mYE-4sfs-1fXv5HhOM-iG5SgWoUxrTwg.02gvpFbMyc843a0x5LmANCtIK_s_WP0LKqOvqmSGV-Ig.PNG.angelcup2001/add+status.png?type=w773)  
  
  
**commit :** `git commit -m "메세지"` 명령어를 통해 파일을 커밋할 수 있습니다. 파일이 스테이징되지 않았다면 커밋을 할 수 없습니다. **git commit -a**옵션을 사용하면 스테이징을 생략하고 바로 커밋을 하는 것도 가능합니다. 
  
  
![first_commit](https://postfiles.pstatic.net/MjAyMTA1MDhfNzUg/MDAxNjIwNDY5ODM1OTQ2.AcSlPYAan-a3b-lHqGO6JnBfFovjSxO4nGhuKC942KUg.qLDzQeVDmqYQmo6joh-Iush9M2U1YS4a18F2-II950gg.PNG.angelcup2001/first_commit.png?type=w773)  

---

### **2. second commit**  
**wrongfile 생성 :** 과제를 작성하면서 더 깔끔하게 작성하고 싶어서 다른 파일을 하나 생성했습니다. 그런데 새 파일에서 작성하다보니 처음 파일이 더 깔끔한 것 같아서 처음 상태로 되돌아가려고 합니다.  
  
  
![wrongfile](https://postfiles.pstatic.net/MjAyMTA1MDhfMTkz/MDAxNjIwNDY5ODQ3MTU0.nQ_xdgIQYWr3hehWOzIRYLUQxc6zyicR8ktC13DeTYUg.A-o1ps52kjrrzSXC0KBPLtgBWaUBUmD466IYja9K3SIg.PNG.angelcup2001/wrongfile.png?type=w773)  
  
  
**log :** 우선 처음 커밋부분으로 되돌아가기 위해서 그 시점을 알아야 하는데 `git log` 명령어를 통해 저장소의 커밋 히스토리를 시간순으로 보여줍니다. 가장 최근의 커밋이 가장 먼저 나옵니다. 그리고 이어서 각 커밋의 SHA-1 체크섬, 저자 이름, 저자 이메일, 커밋한 날짜, 커밋 메시지를 보여줍니다.  
  
  
![log](https://postfiles.pstatic.net/MjAyMTA1MDhfODAg/MDAxNjIwNDY5ODU5MTkz.UK5KFQ43iyPDo0q5kxZBQ3fNV2AqD4-waH8bazr1lH0g.xjtIRn3BT-HQeh6mNBhiAVN88I2MVa3C2dXl4OouIr8g.PNG.angelcup2001/log.png?type=w773)  
  
  
**reset --hard :** log 부분에서 돌아가려고 하는 시점의 일련번호중 앞 6자리를 복사해 옵니다. 그 다음 `git reset 일련번호6자리 --hard` 명령어를 통해 일련번호 전까지 커밋했던 정보들을 삭제할 수 있습니다. 이 명령어를 사용하면 그 전까지의 내용이 모두 삭제되기 때문에 사용에 유의해야 합니다.  
  
  
![reset_--hard](https://postfiles.pstatic.net/MjAyMTA1MDhfMjg5/MDAxNjIwNDY5ODc3NDU4.riBtrJ83DkeaAjCic8idUy46fAR7qifEmTyP5AwX9sIg.O6-IBiqPAgpkQK3V2VOsCqokWvOoxnfhgXrwiSONEDIg.PNG.angelcup2001/reset_--hard.png?type=w773)  

---

### **3. third commit**  
**tag :** 과제를 작성하던 중 '인용구 표시'(>)에 대해 배우게 되었는데 이것을 활용해 인용구를 사용한 파일과 사용하지 않은 파일을 비교해 더 깔끔한 파일을 사용한다고 가정합니다. 우선 원조 파일을 기억하기 위해 태그를 답니다. `git tag 태그메세지` 명령어를 통해 태그를 달 수 있습니다. 보통 버전 표시를 할 때 많이 사용합니다. 그냥 **git tag** 명령어를 입력하면 현재 태그 리스트를 볼 수 있습니다.  
  
  
![tag](https://postfiles.pstatic.net/MjAyMTA1MDhfNTYg/MDAxNjIwNDY5ODg1NDkx.OhPeOdXFJ8T2hECajs3YghlB0xJsA8LmiuULspUZrW0g.NhdcMGM1bm1wrt1w5ffv4NmXyGomd1_ewjuXTTJXewAg.PNG.angelcup2001/tag.png?type=w773)  
  
  
**branch :** `git branch 브랜치이름` 명령어를 통해 브랜치를 생성할 수 있습니다. 쉽게 말하면 가지가 돋아나는 것과 비슷합니다. 이 브랜치를 통해 master 브랜치의 파일을 똑같이 가져올 수 있습니다. 각각의 브랜치는 다른 브랜치의 영향을 받지 않기 때문에, 여러 작업을 동시에 진행할 수 있습니다.  
  
  
**checkout :** `git checkout 브랜치이름` 명령어를 통해 그 브랜치로 넘어갈 수 있습니다.  
  
  
![branch+checkout](https://postfiles.pstatic.net/MjAyMTA1MDhfMjkw/MDAxNjIwNDY5OTA3MjA5.Ej38i2Ez-SZxBMtGgdD6-KEbg3wKAa8OdZVz-NBJ9Ikg.MHe7CSxI4kX-4Lqm75Ep8eSMMF4Zh3Qx0ZDiMJKE5jIg.PNG.angelcup2001/branch+checkout.png?type=w773)  
  
  
**Blockquotes 파일 생성 :** 인용구를 사용한 파일인 Blockquotes 파일을 생성해서 add 명령어로 스테이징을 한 뒤 커밋해줍니다.  
  
  
![Blockquotes](https://postfiles.pstatic.net/MjAyMTA1MDhfODMg/MDAxNjIwNDY5OTE4NTQ1.ZRH4KgoXiuO0IY8zE4KLq2D2iCNk-08ln9gFApNlliUg.I8htAiRemA4PcVXXyIOGsI6v5cSePMQie6OtooIpnEQg.PNG.angelcup2001/Blockquotes.png?type=w773)  
  
  
![add+commit_Blockquotes](https://postfiles.pstatic.net/MjAyMTA1MDhfMjkw/MDAxNjIwNDY5OTM4MDM0.-IVu_DdhZugwcA7JnRgSW-sXp2RXvyYphxXCjYH4otIg.TdPLgcvooIR1G9D1LIMXH8tncBR0PkQL1lDuuwRokh0g.PNG.angelcup2001/add+commit_Blockquotes.png?type=w773)  

---

### **4. fourth commit**  
**code 파일 생성 :** Blockquotes 파일을 작성하던 중에 '코드 표시(`코드`)'에 대해 배우게 되었습니다. 이것도 활용한다고 가정합니다. 우선 code 파일을 생성해 스테이징한 뒤 커밋해줍니다.  
  
  
![add+commit_code](https://postfiles.pstatic.net/MjAyMTA1MDhfMTI1/MDAxNjIwNDY5OTQ3NDgw.qmN1lxMKtO64FfNvEdNOCk8vGIUJtI_lKOJDwfWqipsg.TOK69IPgf4c8u8s03EKRCdsm6iRk_qvz4khn4H2S0OAg.PNG.angelcup2001/add+commit_code.png?type=w773)  
  
  
**merge :** `git merge 브랜치이름` 명령어를 통해 현재 브랜치에 '브랜치이름' 브랜치를 병합할 수 있습니다. 그러므로 checkout 명령어를 통해 Blockquotes 파일로 되돌아간 뒤 명령어를 사용해줍니다.  
  
  
![merge](https://postfiles.pstatic.net/MjAyMTA1MDhfMzQg/MDAxNjIwNDY5OTY4Nzc5.VWlB0VHIQK8vM0K9E8ihW1XhwjCr3NvJdZrvCXQUXxAg.50QkqZEf219TiE4Bi-iJzd_qKiSwhzBiXUUgNV7oChcg.PNG.angelcup2001/merge.png?type=w773)  

---

### **5. fifth commit**  
**rebase :** 'fifth commit'과 'sixth commit'의 순서를 바꾼다고 가정했을 때 `git rebase 일련번호 -i` 명령어를 통해 해결할 수 있습니다. 바꾸고 싶은 곳 전의 일련번호 앞 6자리를 복사해서 명령어를 사용하면 이미지와 같은 창이 나올 것입니다. 두 파일의 이름을 서로 바꾸면 실제로 바뀌고, pick 대신 reword로 고친 후 그 커밋의 메세지를 수정할 수도 있습니다.  
  
  
![rebase_-i](https://postfiles.pstatic.net/MjAyMTA1MDhfMTQy/MDAxNjIwNDc5MzY5Njkx.OqV3Lcnvmj_SNccOkeeCngIAZwQW_x0ml6U8R7Lp1hcg.80tDIMO22QhEPSSfzWL8kWZ4r0Xht-78YUPB6ZPU788g.PNG.angelcup2001/rebase_-i.png?type=w773)  
  
  
![rebase_upsidedown](https://postfiles.pstatic.net/MjAyMTA1MDhfMjAg/MDAxNjIwNDc5Mzg3Nzkw.RuuEnpy23T9_ULOpddkikdvbVYSH_nNpb855tuigby4g.qlLKC-wtl3ENwdYAOlXnzRqJPjoqj7QoxBecdLUFLa0g.PNG.angelcup2001/rebase_upsidedown.png?type=w773)  
  
  
**remote :** 그 다음엔 원격 저장소인 github에 연결을 하기 위해서 `git remote add origin URL` 명령어를 사용합니다. 'origin'은 repository의 이름이며, 다른 이름으로 설정하는 것도 가능합니다.  
  
  
![remote](https://postfiles.pstatic.net/MjAyMTA1MDhfOTAg/MDAxNjIwNDc5Mzk2MzI4._p5HQmhks5vLmapXCWWOFep2FtHKu9I6dE7lFscyvs4g.j-e7kuf9Ptn5gRqhcVAyqO65dHXSlJmIUcI2WAVi2xYg.PNG.angelcup2001/remote.png?type=w773)  
  
  
**pull :**  그 다음 `git pull origin master` 명령어를 통해 원격저장소 변경 사항을 받아옵니다. 다른 작업 환경이나 위치에서 작업할 때, 혹은 공동 작업에서 타인이 커밋해서 이력이 변경되었을 경우 등의 경우가 있습니다. 따라서, pull을 통해서 가져온 후, 작업을 진행하는 것이 좋습니다.  
  
  
![pull](https://postfiles.pstatic.net/MjAyMTA1MDhfODIg/MDAxNjIwNDc5NDA4ODQz.NUj7rduxht90-cjiBRMN6MCGO8Dk9l0Hcn06jkopxKgg.veo2JssCjwLevAE87dBP6R-5ut568-gnN0vQgXlsP0Mg.PNG.angelcup2001/pull.png?type=w773)  
  
  
**push :** 마지막으로 `git push origin master` 명령어를 통해 지금까지 커밋한 이력이 깃허브 repository에 저장됩니다. 깃허브 아이디와 비밀번호를 입력하는 팝업창이 뜨는데 입력에 성공하면 자동으로 저장이 됩니다.  
  
  
![push](https://postfiles.pstatic.net/MjAyMTA1MDhfMTE1/MDAxNjIwNDc5NDE3MTMw.Lh_FOfQpKxumkq5QGBABchuCymTk5zM7wRM5rCLlk3gg.gVFnf_irRv6e8mKYiSo6fEjq7CsC_F3T3rqUukaQmjog.PNG.angelcup2001/push.png?type=w773)  

---

### **6. 명령어 사용 표**  

|명령어|사용 여부|사용 위치|
|---|---|---|
|add|o|[first-commit](#first-commit)|
|branch|o|third commit|
|checkout|o|third commit|
|clone|o|first commit|
|commit|o|fisrst commit|
|config|o|first commit|
|init|o|first commit|
|log|o|second commit|
|merge|o|fourth commit|
|pull|o|fifth commit|
|push|o|fifth commit|
|rebase|o|fifth commit|
|remote|o|fifth commit|
|reset --hard|o|second commit|
|status|o|first commit|
|tag|o|third commit|
