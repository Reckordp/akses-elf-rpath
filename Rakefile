#!/usr/bin/env ruby

desc "Compile"
task default: nil do
	sh 'gcc -shared penyapa.c -o libpenyapa.so'
	sh 'gcc sapaan.c -o sapa -L . -lpenyapa -Wl,-rpath=\'$ORIGIN\''
	sh './sapa'
end