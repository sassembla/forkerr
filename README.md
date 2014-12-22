forkerr


	fork TopLevel {
		entry: {
			fork SecondLevel {
				a: {

				}
				b: {

				}
				c,d: {

				}
				withComment:comment {

				}
				willMerge: {
					merge TopLevel
				}
				_:{

				}
			}
		}
		_: {
			merge exit
		}
	}

これを、フロー図にする。

・fork単位で線の発信点になる  
・merge単位で既存の(あるいは未知の)forkPointに合流する。  

:前の要素はidentifierで、{}内の各要素は階層 + a みたいにidentifyされる。  
fork keyword のうしろに来るのが level identifier  
merge keyword のうしろに来るのも、level identifier  

コンパイルしてASTで扱えるような形に出来れば良くて、カッコ無しとかでもいけると良いなあ。  


実験。
