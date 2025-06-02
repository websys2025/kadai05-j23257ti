## 外部APIの呼び出しのミニレポート
### Q3-1. 郵便番号APIについて説明せよ。
* エンドポイントと機能
* https://zipcloud.ibsnet.co.jp/api/search
* 入力された郵便番号を取得し、住所を検索し、出力する。
*
* リクエストとレスポンスのフォーマット
* リク
* https://zipcloud.ibsnet.co.jp/api/search?zipcode=0790177　（0790177で検索する場合）
*
* レス
* {
	"message": null,
	"results": [
		{
			"address1": "北海道",
			"address2": "美唄市",
			"address3": "上美唄町協和",
			"kana1": "ﾎｯｶｲﾄﾞｳ",
			"kana2": "ﾋﾞﾊﾞｲｼ",
			"kana3": "ｶﾐﾋﾞﾊﾞｲﾁｮｳｷｮｳﾜ",
			"prefcode": "1",
			"zipcode": "0790177"
		},
		}
  },
	"status": 200
}

### Q3-2. 各自で調査したAPIについて説明せよ。
* APIの名称と参照URL
* The Cat API
* https://thecatapi.com/
* エンドポイントと機能
* https://api.thecatapi.com/v1/images/search
* ボタンを押すと、ランダムに猫の画像を出力するもの
* リクエストとレスポンスのフォーマット
* リク
* https://api.thecatapi.com/v1/images/0XYvRd7oD

* レス
* {
"id":"0XYvRd7oD",
"width":1204,"height":1445,
"url":"https://cdn2.thecatapi.com/images/0XYvRd7oD.jpg",
"breeds":[{
  "weight":{"imperial":"7  -  10","metric":"3 - 5"},
    "id":"abys","name":"Abyssinian",
    "temperament":"Active, Energetic, Independent, Intelligent, Gentle",
    "origin":"Egypt",
    "country_codes":"EG",
    "country_code":"EG",
    "life_span":"14 - 15",
    "wikipedia_url":"https://en.wikipedia.org/wiki/Abyssinian_(cat)"
}]

### Q3-3. 感想
* 今回の課題で苦労したこと
* JavaScript からAPIの参照処理コードの作成
* 
* 演習を通して理解できたこと
* 会員登録の住所検索などは、APIを利用して行われていること
* 知らないだけで、現在作成されているホームページには頻繁にAPIが利用されている。
*
* Web APIの利便性や課題など
* 今までのプログラムで複雑化していた、外部のデータとの連携や共有がAPIを利用することで簡単に行える。
* APIの導入が少し複雑であるのと、外部にアクセスすることによっての漏洩被害や、アクセス負荷の対処が今後の課題だと考える。
