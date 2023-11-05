# Natural_Language_Processing_Question_Answering

Bu kod, kullanıcıdan adını ve belirli konular hakkında bilgi almak isteyip istemediğini sormak için bir döngü içeren basit bir etkileşimli programı temsil ediyor. Kullandığı kütüphane, Hugging Face'in Transformers kütüphanesidir, bu kütüphane özellikle doğal dil işleme (NLP) ve makine öğrenimiyle ilgili modelleri ve işlevleri kolayca kullanmanıza olanak tanır. Bu kod, özel bir model ve belirli bir soru-cevap işlemi için bir dönüştürücü (tokenizer) seçmek için Hugging Face'in Transformers kütüphanesini kullanır.

İşte bu kodun temel işlevselliği:

İlgili kütüphaneler ve modeller içe aktarılır: Hugging Face Transformers kütüphanesinden pipeline, AutoModelForQuestionAnswering, ve AutoTokenizer sınıfları içe aktarılır. Ayrıca, bir model ve bir dönüştürücü (tokenizer) belirlenir.

**Kullanıcı ile etkileşim: Bir döngü kullanılarak kullanıcıdan adı alınır (name) ve yapay zeka hakkında bilgi almak isteyip istemediğini sormak için "Evet/Hayır" şeklinde bir soru sorulur (request).**

Kullanıcının cevabına göre bilgilendirme yapılır: Kullanıcı "Evet" derse, yapay zeka ile ilgili genel bilgi verilir. Ardından kullanıcıdan bir soru alınır ve bu soru, belirtilen bağlam ("context") içinde cevaplanmaya çalışılır. Cevap, question_answerer kullanılarak bulunur ve ekrana yazdırılır.

Dünya nüfusu hakkında bilgi alma isteği: Aynı şekilde kullanıcıya dünya nüfusu hakkında bilgi almak isteyip istemediği sorulur (request2). Kullanıcı "Evet" derse, dünya nüfusu ile ilgili genel bilgi verilir ve kullanıcıdan bir soru alınır. Bu soru, belirtilen bağlam içinde cevaplanmaya çalışılır.**

Kullanıcıya çıkış seçeneği sunulur: Kullanıcıya başka bir soru sormak veya programdan çıkmak isteyip istemediği sorulur. "q" tuşuna basarsa, program döngüyü sonlandırır ve çıkar.

Cevaplar ve bilgilendirmeler ekrana yazdırılır: Kullanıcıya sorulan sorulara verilen cevaplar ve bilgilendirmeler, ekrana yazdırılır.

Döngü devam eder veya program sona erer: Kullanıcı başka bir soru sormak isterse veya çıkmak isterse programın davranışı buna göre ayarlanır.
