require 'rake/clean'

task default: :html

desc 'build html'
task :html do
  sh 'review-compile --target=html --all'
end

desc 'build pdf'
task :pdf do
  sh 'review-pdfmaker config.yml'
end

desc 'build epub'
task :epub do
  sh 'review-epubmaker config.yml'
end

CLEAN.include(['*.pdf', '*.epub', '*.html', '*.xml'])
