#!/usr/bin/env rake

task default: :markdown

ORG = Rake::FileList.new('**/*.org') do |files|
  files.exclude do |file|
    `git ls-files #{file}`.empty?
  end
end

task markdown: ORG.ext('md')

rule '.md' => '.org' do |task|
  sh "pandoc #{task.source} -t markdown_github -o #{task.name}"
end
