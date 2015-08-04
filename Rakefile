require 'rake/clean'

CLEAN.include '*.aux'
CLEAN.include '*.log'
CLEAN.include '*.out'

task :default => 'poster.pdf'

CLOBBER.include 'poster.pdf'

rule '.pdf' => '.tex' do |t|
  sh "pdflatex #{t.source}"
end
