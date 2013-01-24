$: << File.join(Dir.getwd, 'lib')

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

  puts Opal::Handlebars.new.compile(content)
end
