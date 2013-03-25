require 'bundler'
Bundler.require

$: << File.expand_path('../lib', __FILE__)
require 'opal/handlebars'

desc "REMOVE THIS"
task :handlebars do
  content = <<-HTML
    <div class="adam">
      {{surname}}
    </div>
    Email: {{text_field email limit="400"}}

    {{{unescaped_content}}}

    {{#if author}}
      {{author.name}}
    {{/if}}
  HTML

  puts content
  puts "\n----\n\n"
  puts Opal::Handlebars.new.compile(content)
end


#require 'opal/spec/rake_task'
#Opal::Spec::RakeTask.new(:default)
