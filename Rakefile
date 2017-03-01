# encoding: utf-8
require 'bundler'
Bundler::GemHelper.install_tasks

require 'rspec/core/rake_task'

namespace :spec do
  RSpec::Core::RakeTask.new('unit') do |t|
    t.pattern = 'spec/etcd/*_spec.rb'
  end

  RSpec::Core::RakeTask.new('integration') do |t|
    t.pattern = 'spec/integration/*_spec.rb'
  end
end

task default: 'spec:unit'
